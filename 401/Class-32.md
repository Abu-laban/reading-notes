## Context API - Behaviors

### Review, Research, and Discussion

**1. When you have multiple contexts, what component type should you use (class/function) and why?**

The static contextType property won’t work if you need more than one, so instead you need to use a context consumer.

**2. What are some good use cases for using the Context API for global state?**

when some data needs to be accessible by many components at different nesting levels.

**3. How can you best test context?**

The best way to test Context is to make our tests unaware of its existence and avoiding mocks. We want to test our components in the same way that developers would use them (behavioral testing) and mimic the way they would run in our applications (integration testing).


**Term** | **Definition**
-----|-----
context | context is related to objects. It refers to the object to which a function belongs. When you use the JavaScript “this” keyword, it refers to the object to which function belongs.
useContext() | useContext” hook is used to create common data that can be accessed throughout the component hierarchy without passing the props down manually to each level.
static context | Static context defines items that are needed to prepare executables, items such as the names and types of external variables and functions that will be available at run time as well as compilation modes like backwards compatibility, math mode, and so on.
