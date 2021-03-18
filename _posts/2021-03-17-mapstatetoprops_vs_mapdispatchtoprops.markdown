---
layout: post
title:      "mapStateToProps vs mapDispatchToProps"
date:       2021-03-18 03:53:20 +0000
permalink:  mapstatetoprops_vs_mapdispatchtoprops
---


Connect is a powerful function provided by react-redux. Connect typically receives 2 parameters, mapStateToProps and mapDispatchToProps. These parameters allow programmers to customize the data that their components receive and reutilize functionality. 

mapStateToProps is the conventional name given to a function in a React component to allow the component to access information in the global Redux store. Any component which needs access to information in the Redux store and cannot directly receive them as props can be connected to the Redux store to receive read-only information from the store as props.

mapDispatchToProps is the conventional name given to a function in a React component to allow the component to update the global Redux store. Any component connected to the Redux store using connect will have access to dispatch by default. From here, users can create actions and dispatch them through their specific reducer. A reducer is a function which takes in an action object, typically containing type and payload keys. Reducer functions result in an updated state, triggering components re-render. By using mapDispatchToProps, a component can use its own local events to trigger updates to the Redux store, passing valuable information throughout the application. 

In my recent project TopShelf, I have a component RandomItem which displays information about a random item. To do this, I generate a random number within the length of my total number of item, provided via mapStateToProps. This allows me to get a single item from the list:

```
const randomItem = this.props.items[Math.floor(Math.random() * this.props.items.length)];
```

This is accomplished by accessing the Redux store and getting the items array:

```
const mapStateToProps = state => {
    
    return {items: state.items}
}
```

Connecting components when neccessary allows applications to be more cohesive, less repetitive, and allows each component to focus on its own concerns. 




