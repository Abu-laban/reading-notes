# In memory storage

## Understanding the JavaScript Call Stack

1. What is a ‘call’?

> is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).

2. How many ‘calls’ can happen at once?

The browser (hosting environment) has a **maximum** stack call that it can accomodate before throwing a stack error.

> the browser throws a **“Maximum call size exceeded”**.

3. What does LIFO mean?

> Last In, First Out data structure.

>       it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

4.  Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

        function firstFunction(){
        console.log("Hello from firstFunction");
        }

        function secondFunction(){
        firstFunction();
        console.log("The end from secondFunction");
        }

        secondFunction();

> Hello from firstFunction

> The end from secondFunction

5. What causes a Stack Overflow?

> A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

## JavaScript error messages

1. What is a ‘refrence error’?

> This is as simple as when you try to use a variable that is `not yet declared` you get this type os errors.

    console.log(foo) // Uncaught ReferenceError: foo is not defined

> This is also a common thing when using `const` and `let`, they are hoisted like `var` and `function` but there is a time between the hoisting and being declared so when you try to access them a reference error occurs, the fact that this happens to `let` and `const` is called **Temporal Dead Zone (TDZ)**.

        foo = 'Hello' // Uncaught ReferenceError: foo is not defined
        let foo

2. What is a ‘syntax error’?

> This occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

    JSON.parse( {'foo': 'bar'} ) // Uncaught SyntaxError: Unexpected token o in JSON at position 1

>       Some syntax errors like sending a trailing comma when calling a function are handled without error by most recent browsers, but older ones you have to be careful.

3. What is a ‘range error’?

> Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.

    var foo= []
    foo.length = foo.length -1 // Uncaught RangeError: Invalid array length

4. What is a ‘tyep error’?

> this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

        var foo = {}
        foo.bar // undefined
        foo.bar.baz // Uncaught TypeError: Cannot read property 'baz' of undefined

**This is probably the most frequent error in JS**

5. What is a breakpoint?

The breakpoint can also be achieved by putting a debugger statement in your code in the line you want to break.

> which will make your program stop at that point only if a condition is met, this is awesome for when you want to debug huge cycles for specific values.

6. What does the word ‘debugger’ do in your code?

> To identify JavaScript errors and we can use it for example to debug huge cycles for specific values.
