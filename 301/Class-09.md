# FUNCTIONAL PROGRAMMING

1. What is functional programming?

>       Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.

2. What is a pure function and how do we know if something is a pure function?

>       Pure functions are stable, consistent, and predictable. Given the same parameters, pure functions will always return the same result. We don’t need to think of situations when the same parameter has different results — because it will never happen.

3. What are the benefits of a pure function?

> The code’s definitely easier to test. We don’t need to mock anything.

- They’re easier to reason about
- They’re easier to combine
- They’re easier to test
- They’re easier to debug
- They’re easier to parallelize

4. What is immutability?

> Immutables are the objects whose state cannot be changed once the object is created. Strings and Numbers are Immutable.

5. What is Referential transparency?

>       Basically, if a function consistently yields the same result for the same input, it is referentially transparent.

`pure functions + immutable data = referential transparency`

> Referential transparency and referential opacity are properties of parts of computer programs. An expression is called referentially transparent if it can be replaced with its corresponding value (and vice-versa) without changing the program's behavior.

# Modules and require()

1. What is a module?

>       Module in Node. js is a simple or complex functionality organized in single or multiple JavaScript files which can be reused throughout the Node. js application. Each module in Node. js has its own context, so it cannot interfere with other modules or pollute global scope.

2. What does the word ‘require’ do?

method is used to load and cache JavaScript modules. So, if you want to load a local, relative JavaScript module into a Node. js application, you can simply use the `require()` method.

`require()` is used to consume modules. It allows you to include modules in your app. You can add built-in core Node.js modules, community-based modules (node_modules), and local modules too.

>       The basic functionality of require is that it reads a JavaScript file, executes the file, and then proceeds to return the exports object. It is worth noting that each time you subsequently require an already-required file, the exports object is cached and reused.

3. How do we bring another module into the file the we are working in?

> by creating a JavaScript file. Every time you create a new file with .js extension, it becomes a module.

4. What do we have to do to make a module available?

The first thing you do to get access to module features is export them. This is done using the export statement.

> Basiclly export it by useing module.export.
