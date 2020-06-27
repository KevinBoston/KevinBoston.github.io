---
layout: post
title:      "A glass of WhisCLI for the journey - My CLI project"
date:       2020-06-27 18:55:49 +0000
permalink:  a_glass_of_whiscli_for_the_journey_-_my_cli_project
---




My independent Command Line Interface project, the culminating project for the first section of Software Engineering bootcamp, presented challenges regarding both direction and scope. Initially, I designed a more ambitious project than fit the logistic parameters allotted, but successfully reframed my project to meet my goals. I gained insight about balancing project scope with resources available, and learned to rely on and work with others to proofread code and suggest improvements and changes to logic.

Beginning the project came with its own set of challenges. I initially planned do the work in a local development environment, but proceeding  in the Learn.co IDE proved the best use of time. This decision allowed me to make progress, but resulted in several crashed sessions and countless lines of lost code which took more hours to recreate. I learned from the constant crashes, saving more often as well as doing occasional offline work when slowly creating new code. In the end, getting a sequence of code working and losing it led me to repeat the development process, providing me with further practice and leading to better code.

My project, WhisCLI, scrapes liquorama.net, a site which I had not used before this project. I set out to find a website with a well-organized store, but with limited enough design to lend itself to straightforward scraping. I used my knowledge of whisky to determine properties that a whisky object should have, namely alcohol content, age statement, and country of origin, but eventually modified this approach to better align with available content.

I initially intended to generate my categories from the website, scraping the homepage (BASEURL in the project) and searching through a side menu to find all category headers with the text *whisk*, after a discussion with my cohort lead, I elected to remove this feature, and re-oriented my project plan accordingly.

With a more narrowed scope, I was well situated to progress with the project. I scraped the category pages to provide a list of whisky objects and access a name, URL, category, description, and price for each object. The objects behave much like the webpages they are scraped from, with a few minor functionality discrepancies based around the nature of the specific data I am accessing.

I am satisfied with the accomplishment of conceptualizing and creating a project on my own and think that the skills I have learned on this project, including planning, scraping, and refactoring, will be invaluable in the coming modules.
