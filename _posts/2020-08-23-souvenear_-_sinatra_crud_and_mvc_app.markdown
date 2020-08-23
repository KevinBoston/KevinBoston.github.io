---
layout: post
title:      "Souvenear - Sinatra, CRUD, and MVC app"
date:       2020-08-23 12:34:16 +0000
permalink:  souvenear_-_sinatra_crud_and_mvc_app
---


One of my favorite aspects of travel is remembering interesting aspects of the trip. I have a map where I record locations and make notes about past vacations and what I brought back. Souvenear is the natural outcome of digitizing this process. Souvenear is an MVC app featuring CRUD with both a trip model and a souvenir model. Users are able to sign up and login, creating records of trips and souvenirs that appear on their account page. In addition, users can be administrators, which allows users to see a full list of all recorded trips, rather than only their own. I learned how to better set up ActiveRecord migrations (and about the dangers of extra white space), as well as how to test the project using the Shotgun gem.

The basic project requirements stipulated that I create a project that includes both a user model and a second model with full CRUD functionality. Through this project I developed a deeper understanding of Sinatra, ActiveRecord, and Sqlite concepts. In keeping with the object-oriented philosophy of modeling real objects, I wanted the application to be able to keep track of multiple souvenirs associated with each trip, and to be able to keep track of multiple trips. Thus, I decided to develop a relationship structure in which users have many souvenirs through trips.

I finished the main structure of the project early in the project cycle, which enabled me to spend time developing additional features, spurred on by curiosity. One idea that struck me early on was to add a view that would toggle an admin function on, allowing the admin user to have an expanded view beyond their own trips and souvenirs. This feature manifested itself on the /users/make_admin/ view, giving users the option to toggle admin rights on or off.

Along the way, I encountered several bugs that I found particularly challenging. First, I encountered an issue setting up my databases through migrations. After an unreasonable amount of time, I discovered that extra white space doesn’t agree with ActiveRecond and Sqlite. Once I made it past this issue, I began testing the functionality of my views using shotgun and rackup. There, I encountered two instances of shotgun running at the same time. With two terminals running, I couldn’t see the output I needed for debugging. Returning to one shotgun server solved this error, which enabled me to complete the project.

Overall, Souvenear allowed me to engage my curiosity and to test my limits as a software engineer. I started with a goal that was personal to me and was able to follow through with the more complex version of the program I had envisioned. Once there, I had the opportunity to add further features and to devote time to tinkering and experimenting with various features and gems. The bugs provided the icing on the cake for what I am told is the lifelong experience of software developers: spending hours searching for a technical solution to a typo. I genuinely enjoyed this project, and look forward to the next.
