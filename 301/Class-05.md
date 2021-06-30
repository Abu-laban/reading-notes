# Thinking in React

React is, in our opinion, the premier way to build big, fast Web apps with JavaScript. It has scaled very well for us at Facebook and Instagram.

## Break The UI Into A Component Hierarchy

The first thing you’ll want to do is to draw boxes around every component (and subcomponent) in the mock and give them all names. If you’re working with a designer, they may have already done this, so go talk to them! Their Photoshop layer names may end up being the names of your React components!

![Break](https://res.cloudinary.com/practicaldev/image/fetch/s--YQRzFDyP--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/1q15ngywa5fxcbaho6uf.PNG)

> But how do you know what should be its own component?

Use the same techniques for deciding if you should create a new function or object. One such technique is the **single responsibility principle**, that is, a component should ideally only do one thing.

If it ends up growing, it should be decomposed into smaller subcomponents.

![single](https://www.logiqlabs.com/wp-content/uploads/2021/04/SRP.png)

## Build A Static Version in React

![static](https://cdn.cosmicjs.com/170044f0-5f53-11eb-852b-43268d756f2e-Static-Site-Generation.png)

> To build a static version of your app that renders your data model, you’ll want to build components that reuse other components and pass data using props.

props are a way of passing data from parent to child. If you’re familiar with the concept of state, **don’t use state at all** to build this static version. State is reserved only for interactivity, that is, data that changes over time. Since this is a static version of the app, you don’t need it.

The components will only have `render()` methods since this is a static version of your app.

The component at the top of the hierarchy `(FilterableProductTable)` will take your data model as a prop.

If you make a change to your underlying data model and call `ReactDOM.render()` again, the UI will be updated. You can see how your UI is updated and where to make changes. React’s one-way data flow (also called one-way binding) keeps everything modular and fast.

## Let’s go through each one and figure out which one is state. Ask three questions about each piece of data:

1. Is it passed in from a parent via props? If so, it probably isn’t state.

2. Does it remain unchanged over time? If so, it probably isn’t state.

3. Can you compute it based on any other state or props in your component? If so, it isn’t state.

## Identify Where Your State Should Live

> Remember: React is all about one-way data flow down the component hierarchy. It may not be immediately clear which component should own what state. `This is often the most challenging part for newcomers to understand`, so follow these steps to figure it out:

For each piece of state in your application:

- Identify every component that renders something based on that state.

- Find a common owner component ,(a single component above all the components that need the state in the hierarchy).

- Either the common owner or another component higher up in the hierarchy should own the state.

- If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.
