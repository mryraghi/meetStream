# meetStream
Academic project that aims to consume a stream of live data into some 3d data representation.

---
## Project proposal
## Preamble
We noticed that usually students, while developing projects for university courses, tend to emulate existing projects. For example, classical projects are the travel agency assistant or the e-shop. Though, we think that due to the inner structure of the course of study at university and due to difficulties related to time and knowledge, student projects are not comparable to “real-life projects” both in complexity and efficiency.
This is the reason why we decided to develop a new and creative project.

---
## Project Description
As introduced in the previous paragraph, our project wants to be something fancy and amusing. It consists in showing to the user in a nice and cool way live data from an external source. Our source of data is the "Meetup" API. What we are going to download from this source is an always updating list of events around the world of the most various topics.  We are going to get the live data stream from this source, parse it and show it to the user. Moreover it will be possible to filter the data by topic and by geographical area.
Finally, we should say that even if our idea is not supposed to have any practical use, we can identify some side effects. In fact, it may be a fast and easy way for checking for events in a particular city or area.

---
## Project Structure
### Server application
Retrieves live streaming from the “Meetup” API `http://www.meetup.com/it-IT/meetup_api/docs/`, filters and forwards it to the connected users, according to their requests (For example, “all events in a range of 50 km from a given location”). This trick allows us to add/fix/maintain features without compromising the client application, keeping it atomic towards the datasource possible changes.

* **languages**: mainly Elixir, source: `http://elixir-lang.org/`
* **frameworks**: phoenix, used as: interface between the web and our application

### Client application
Opens a socket connection with our API service and displays live data to the user.

* **languages**: mainly js, html5 and css3
* **libraries**: d3, source `https://github.com/d3/d3/`, used to: data display



