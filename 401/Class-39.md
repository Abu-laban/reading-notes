# Redux - Additional Topics

## Review, Research, and Discussion

### What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?

Best practice would be to fire off an api call from a useEffect() call on pageload. Because this is asynchronous, this will require Thunk middleware. You may then  use mapStateToProps() to assign the returned data to props which can be passed to the component in question. [src](https://stackoverflow.com/questions/39356517/correct-way-to-pre-load-component-data-in-reactredux)

### When using a thunk/async action that dispatches the actual action, which do you export from your reducer?

You export the thunk (async) action, which then dispatches the actual action locally.

## Term

**middleware** - code that runs between two functions - in the case of redux, code that is wrapped between our `createStore()` function and our `connect()` function.

**thunk** - a kind of middlware that takes a function, does some processing, and returns another function.

## Preparation Materials

[Redux Toolkit (RTK)](https://redux-toolkit.js.org/)

- [RTK Tutorial](https://redux-toolkit.js.org/tutorials/overview)

### Alternative State Managers

[MobX](https://mobx.js.org/getting-started.html)

[HookState](https://hookstate.js.org/)