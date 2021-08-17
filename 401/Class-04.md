# Data Modeling

## Review, Research, and Discussion

### **Name 3 advantages to Test Driven Development**

- Better program design and higher code quality.
- Code flexibility and easier maintenance.
- TDD reduces the time required for project development.

### **In what case would you need to use beforeEach() or afterEach() in a test suite?**

* If need to setup a mock object or data structure and this object or structure can be reused by all the tests


###  **What is one downside of Test Driven Development**

When feature changes, implementation will change as well, and many test cases will fail

> it slows down development, for rapidly iterative startup environments the implementation code may not be ready for some time due to spending time writing tests first.


### **What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?**

 - ES6 class constructors creates objects by adding function to their prototypes Blueprint.

 - Constructor/Prototype Classes are function constructors also create objects along with inheritance property.

ES6 classes is like a container that holds the constructor and the methods associated with your instantiated object.

``is that a class defines a type which can be instantiated at runtime, whereas a prototype is itself an object instance.``

### **”Why REST?”**

> REST aims to make caching easier. Since the server is stateless and each request can be processed individually, GET requests should usually return the same response regardless of previous ones and the session. This makes the GET requests easily cacheable and browsers usually treat them as such.

---

### *Document the following Vocabulary Terms*

``functional programming``

is the process of building software by composing pure functions, avoiding shared state, mutable data, and side-effects.

``object-oriented programming (OOP)``

is a computer programming model that organizes software design around data, or objects, rather than functions and logic. An object can be defined as a data field that has unique attributes and behavior.

``class``

are a template for creating objects. They encapsulate data with code to work on that data.

``super``

 keyword to call the constructor of the super class.

``this``

In the global execution context (outside of any function), this refers to the global object whether in strict mode or not.


``Test Driven Development``

Test-driven development (TDD) is a software development process relying on software requirements being converted to test cases before software is fully developed

> It is most often associated with automated testing

``Jest``

is a JavaScript testing framework developed by Facebook. It works out of the box with minimal configuration and has in-built test runner, assertion library and mocking support.

``Continuous Integration (CI)``

is the practice of automating the integration of code changes from multiple contributors into a single software project.

``REST``

 is an architectural style that handles the client-server relationship

``Data Model``

the process of visualizing and representing data for storage in a data warehouse. The model is a conceptual representation of the data, the relationships between data, and the rules. The modeling itself can include diagrams, symbols, or text to represent data and the way that it interrelates.