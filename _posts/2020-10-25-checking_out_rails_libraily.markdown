---
layout: post
title:      "Checking Out Rails: Libraily"
date:       2020-10-25 16:58:42 -0400
permalink:  checking_out_rails_libraily
---


Starting Rails after Sinatra was like stepping into a magical world: magical in that way where one doesn’t always comprehend exactly what is happening or what may happen next.

At first I thought I was understanding the patterns, but as time went on I realized I had underestimated Rails’ power and functionality. This led me to much review of course material and necessitated extra hands on learning during my project, all while juggling more external scheduling challenges than usual. Ultimately, this project demanded the use of my problem solving and time management skills in a challenging and rewarding way that previous projects have not.

After completing the Rails Amusement Park lab, I decided on an overall structure for Libraily that featured models for a Library, Book, and User. Users can be librarians (admins) and have typical user attributes as well as a location. Libraries have a name, a location, and have many books. Libraries and their locations serve as a model for actual local library systems, in which one library system may allow users to borrow from several locations. Books have typical attributes. I had originally intended for book to function as a join between Users and Libraries, but eventually elected to create a fourth model: Check Outs. Check Outs features an agreement for the user to 'return' their checked-out books, accepting both a :book_id and :user_id.


During this project cycle I learned about new tools for debugging my project, including ByeBug, and learned better ways to research error messages. I read sizeable quantities of documentation to understand the correct methods to use in the application, and in the end I understood Rails better for having to investigate the causes for errors.

With Libraily, I committed to an idea and persisted to see it through to completion. Through errors, scoping issues, and several late nights, I tested my limits and came to understand the systems behind the magic of Rails. 
