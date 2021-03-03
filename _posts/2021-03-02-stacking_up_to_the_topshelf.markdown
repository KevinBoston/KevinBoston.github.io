---
layout: post
title:      "Stacking up to the TopShelf"
date:       2021-03-03 04:13:48 +0000
permalink:  stacking_up_to_the_topshelf
---




After roughly a year of full time work, full time study, and a pandemic, I could really use a drink; and I'm confident those in my cohort would agree. So, for my final project at Flatiron, I decided to build a React application as a way to catalog celebratory drinks.

TopShelf, named because I’m sure my classmates only drink the best, has a React-Redux frontend connected to a Ruby-on-Rails API backend. Since React is specialized towards separation of concerns, I have many components throughout the application, each of which handles specific tasks. Most components are connected to the Redux store via connect, allowing them to access either User information (displaying the user's username) or Item data. 

I modelled TopShelf with a design standard for a larger website: a main landing page, then a page with various items that act as gateways to further information. The homepage contained many firsts for me, including my first foray into CSS, implementing a styled NavBar, as well as a RandomItem component.

The RandomItem component is an abstracted 'featured' or 'recommended' section. In a fully-developed website, this area may recommend a particularly popular item or promote a sale, for example. As an introduction, I ensured that RandomItem was connected to my Redux store and had access to :items. I generated a random number and passed selected that index from my list of items.

`const randomItem = this.props.items[Math.floor(Math.random() * this.props.items.length)]`

The item's name was placed prominently in the small card, allowing a new user to jump right into an item's view. Every visit to the home page would render a different item, making each page view feel a little different.

Ensuring that the app was working perfectly was a challenge, since managing state and fetching data for the Store asynchronously proved more difficult than I anticipated, but I think that these challenges helped me to better understand the React development cycle. My newfound grasp on React allows me to better see areas where my application can grow, and where I can best utilize React's strengths to build an even stronger application in the future. 
