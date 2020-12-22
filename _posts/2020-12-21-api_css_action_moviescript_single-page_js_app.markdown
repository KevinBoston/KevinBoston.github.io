---
layout: post
title:      "API, CSS, Action! MovieScript: Single-page JS App"
date:       2020-12-22 00:34:16 +0000
permalink:  api_css_action_moviescript_single-page_js_app
---


MovieScript is a single-page JavaScript application with a Ruby-on-Rails API backend. The application renders information persisted by list and then by individual title. Users on the site can create, view, and delete both titles and movies. Lists have many movies and individual movies belong to lists; this allows the front end to access movie data quicker than making a separate fetch request.

The application seemed simple enough during the initial planning stages but proved tricky in implementation. Despite many challenges, I persisted in searching for new approaches to resolving errors and preventing undesirable behavior. In one such instance, the program was duplicating part of the “add a movie” form. After some trouble shooting, I was able to isolate where the function in question was called and prevent the behavior.

During this project, I gained a greater understanding of JavaScript and of the Object-Oriented Framework through extensive debugging and refactoring. Object Orientation helped me solve several problems that could not have been solved using standard functional JavaScript. For example, when users enter information to create a new movie, they must select to which list it belongs. In the early stages of development I had hardcoded the options to the lists I created in my seed file, but this approach would break down as the application grew. The hardcoded approach reached its limit when I decided to add the ability to add lists, but I was able to leverage Object Orientation to dynamically generate this particular form element while maintaining most of the form in standard HTML.

I decided to add a few features designed to make the app more user friendly and streamlined, including buttons to toggle the display of the input forms. I initially intended for users to be able only to delete lists, but upon reflecting on potential user experience concluded it made the most sense to be able to delete both lists and movies.

Ultimately, developing MovieScript provided the impetus to combine the lessons I learned over the previous unit into a functioning project. Honing in on a coding cycle of first building, then testing, and finally refactoring helped me understand what to expect from each individual function.
