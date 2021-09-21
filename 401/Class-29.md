# Advanced State with Reducers

### Review, Research, and Discussion

**1. How can we ensure that an effect hook runs only once?**

>  If we pass an empty array [] , it just renders the component only once like componentDidMount 

**2. Can useState() update more than one state variable at the same time?**

>  You can have multiple states inside of a single component: call multiple times useState()

**3. Is useState() synchronous?**

> no , useState() doesn't update value of the variable if called just after setting value.


Trems|DEF
-----|---
State Hook| A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components. We'll learn other Hooks later.
Component Lifecycle|Every React Component has a lifecycle of its own, lifecycle of a component can be defined as the series of methods that are invoked in different stages of the component's existence. ... A React Component can go through four stages of its life as follows

![](https://media.geeksforgeeks.org/wp-content/uploads/lifecycle_reactjs.jpg)


