# State and Props

# React: Component Lifecycle Events

## What are component lifecycle events?

React lets you define components as classes or functions. The methods that you are able to use on these are called lifecycle events. These methods can be called during the lifecycle of a component, and they allow you to update the UI and application states.

![image](https://miro.medium.com/max/2800/0*0saPKFiTUk6W3FYp)

_Mounting, Updating, and Unmounting are the three phases of the component lifecycle._

1.  _Mounting_

         When an instance of a component is being created and inserted into the DOM it occurs during the mounting phase. Constructor, static getDerivedStateFromProps, render, componentDidMount, and UNSAFE_componentWillMount all occur in this order during mounting.

2.  _Updating_

        Anytime a component is updated or state changes then it is rerendered. These lifecycle events happen during updating in this order.
        static getDerivedStateFromProps, shouldComponentUpdate, render,
        getSnapshotBeforeUpdate, componentDidUpdate, UNSAFE_componentWillUpdate, UNSAFE_componentWillReceiveProps

3.  _Unmounting_

        The final phase of the lifecycle if called when a component is being removed from the DOM. componentWillUnmount is the only lifecycle event during this phase.

`constructor()`

The constructor for a React component is called before it is mounted.If the component is a subclass you should call super(props), or the props will be undefined. constructors can be used to assign state using this.state or to bind event handle methods to an instance.

> Avoid using this.setState() in the constructor because it can lead to side effects, and it is unnecessary. Doing this will ignore all updates to props, so it shouldn’t be done unless it is intentional.

`render()`

Render is the only required method in a class component. It will examine this.props and this.state when called. The render function should not modify the component state because it would cause a lot of bugs by changing the state every time it rerenders. I also should not directly interact with the browser. render will not be invoked if shouldComponentUpdate() returns false.

`componentDidMount()`

This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in componentWillUnmount().

> setState() can be called here, but it should be used sparingly, because it will cause a rerender, which can lead to perfomance issues.

`componentWillUnmount()`

This method allows you to clean up the DOM and netwrok requests/ subscriptions.

# What's the difference between props and state in React?

Let's compare props and state. Here's a definition of each:

`"props"` (short for "properties") is an object of arbitrary inputs a React function component accepts as the first argument.

`"state"` is data that changes over the lifetime of a specific instance of a React component.

## Props

Think of props as arguments to a function. React components are functions which return JSX (or more generally something that's renderable like React elements, null, a string, etc.). Typically when you have a piece of code that you would like to reuse, you can place that code into a function and any dynamic values that code used before can be accepted as arguments

## State

State is data that changes over time.

![image1](https://i.stack.imgur.com/wqvF2.png)

![image2](https://res.cloudinary.com/practicaldev/image/fetch/s--Qr2q1dEA--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/vghwx14ekbmlil1vpi0g.png)
