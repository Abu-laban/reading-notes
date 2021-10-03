# Application State with Redux

## Review, Research, and Discussion

Redux stores all application state in a single javascript object called the state tree. All mutations and changes to the state data object are explicit, so we can keep track of them easily. The state tree is redundant, so we must use an action method to modify the data.

## 1. **What are the advantages of storing tokens in “Cookies” vs “Local Storage”**

Local Storage is vulnerable to XSS attacks, and cookies are automatically attached to every HTTP request on your server. [src](https://blog.cotter.app/localstorage-vs-cookies-all-you-need-to-know-about-storing-jwt-tokens-securely-in-the-front-end/)

## 2. **Explain 3rd party cookies.**

First-party cookies live on the website you are currently visiting. Third-party cookies are created by websites other than the one you are currently visiting. [src](https://us.norton.com/internetsecurity-privacy-internet-privacy-third-party-cookies.html)

## 3. **How do pixel tags work?**

As a pixel loads, it runs associated javascript code which does a given action. In the context of advertising, these often collect and send data back to some third party.

## Document the following Vocabulary Terms

**cookies** - a small piece of data sent from a server to a client, which is then attached to every client request back to that server.

**authorization** - a HTTP request header that contains required authentication credentials.

**access control** - the process of requiring client authenticaion to verify different levels of access on a server.

**conditional rendering** - the process of using React to render certain components or elements based on conditional logic.

## Preparation Materials

[Dan Abramov Redux Tutorials](https://egghead.io/courses/fundamentals-of-redux-course-from-dan-abramov-bd5cc867)

[worlds easiest guide to redux](https://www.freecodecamp.org/news/understanding-redux-the-worlds-easiest-guide-to-beginning-redux-c695f45546f6/)

[testing reducers](https://medium.com/@netxm/testing-redux-reducers-with-jest-6653abbfe3e1)

[Redux Docs](https://redux.js.org/)