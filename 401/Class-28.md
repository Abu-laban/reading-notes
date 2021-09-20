# Component Lifecycle / useEffect() Hook

### Review, Research, and Discussion

**1. Why do we not need more .html pages in a multi-page React app?**

 react apps are single page app ,A React app consists of a single HTML file index.html. The views are coded in JSX format as components.

**2. If we wanted a component to show up on every page, where would we put it and why?**

>  Inside the  < BrowserRouter/ >, outside a < Route/ >, to have it always no matter what the current route is .

**3. What does routing do with the components that were rendered when a new route is requested**

> it goes to the new componetnt and remove the old one _cleans up _

**4. What does props.children contain?**

> children is a special property of React components which contains any child elements defined within the component, e.g. the divs inside Example above. {this.props.children} includes those children in the rendered result.

**5. How do useState() and this.setState() differ?**

* The setState function is used to handle the state object in a React class component.

* setState is merging the previous state with the new one, it means that you dont have to pass the full state object every time you want to change some part of the state. React will update given properties and won't touch the rest. The useState's updater rewrites a previous state with a new one and it does not perform any merging. Its just replacement instead of merging.


Trems|DEF
-----|---
State Hook|     The useState() is a Hook that allows you to have state variables in functional components , it takes the initial state as an argument and returns an array of two entries.
Mounting and Un-Mounting|   The main job of React is to figure out how to modify the DOM to match what the components want to be rendered on the screen. React does so by mounting (adding nodes to the DOM), unmounting (removing them from the DOM), and updating (making changes to nodes already in the DOM).

