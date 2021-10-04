# Redux - Asynchronous Actions

## Review, Research, and Discussion

### 1. **How granular should your reducers be?**

Generally, as granular as possible. This allows for easier organizion, debugging, and testing. It also allows you to more easily add new features or remove features in the future. [src](https://redux.js.org/style-guide/style-guide)


### 2. **Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched**

PRO! Having multiple reducers fire on a shared action is a great way to handle complex state changes in a predicable, reliable, and modular way, as long as it is intended.

### 3. **Name a strategy for preventing the above**

Use explicit names for each action to prevent unintended firing (i.e. don't use 'RESET' for every reducer... unless you want them all to reset at the same time!)

## Document the following Vocabulary Terms

**store** - the object created by redux that stores all states for a given application. This is the single source of truth for our application.

**combined reducers** - a way redux allows us to 'export' many reducer files from a single source to our store, so that they are all available in different parts of an app.

## Preparation Materials

[async actions](https://redux.js.org/tutorials/fundamentals/part-6-async-logic)

[thunk middleware](https://github.com/reduxjs/redux-thunk)

[redux thunk](https://www.digitalocean.com/community/tutorials/redux-redux-thunk)