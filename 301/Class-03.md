# Passing Functions as Props

# Lists and Keys

> First, let’s review how you transform lists in JavaScript.

Given the code below, we use the `map()` function to take an array of `numbers` and double their values. We assign the new array returned by `map()` to the variable `doubled` and log it:

        const numbers = [1, 2, 3, 4, 5];
        const doubled = numbers.map((number) => number * 2);
        console.log(doubled);

This code logs `[2, 4, 6, 8, 10]` to the console.

In React, transforming arrays into lists of `elements` is nearly identical.

## Rendering Multiple Components

You can build collections of elements and `include them in JSX` using curly braces `{}`.

Below, we loop through the `numbers` array using the JavaScript `map()` function. We return a `<li>` element for each item. Finally, we assign the resulting array of elements to `listItems`:

        const numbers = [1, 2, 3, 4, 5];
        const listItems = numbers.map((number) =>
        <li>{number}</li>
        );

We include the entire `listItems` array inside a `<ul>` element, and `render it to the DOM`:

        ReactDOM.render(
        <ul>{listItems}</ul>,
        document.getElementById('root')
        );

This code displays a bullet list of numbers between 1 and 5.

## Basic List Component

Usually you would render lists inside a component.

We can refactor the previous example into a component that accepts an array of `numbers` and outputs a list of elements.

        function NumberList(props) {
        const numbers = props.numbers;
        const listItems = numbers.map((number) =>
        <li>{number}</li>
        );
        return (
        <ul>{listItems}</ul>
        );
        }

        const numbers = [1, 2, 3, 4, 5];
        ReactDOM.render(
        <NumberList numbers={numbers} />,
        document.getElementById('root')
        );

> When you run this code, you’ll be given a warning that a key should be provided for list items. A “key” is a special string attribute you need to include when creating lists of elements. We’ll discuss why it’s important in the next section.

Let’s assign a `key` to our list items inside `numbers.map()` and fix the missing key issue.

        function NumberList(props) {
        const numbers = props.numbers;
        const listItems = numbers.map((number) =>
        <li key={number.toString()}>
        {number}
        </li>
        );
        return (
        <ul>{listItems}</ul>
        );
        }

        const numbers = [1, 2, 3, 4, 5];
        ReactDOM.render(
        <NumberList numbers={numbers} />,
        document.getElementById('root')
        );

## Keys

Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity:

        const numbers = [1, 2, 3, 4, 5];
        const listItems = numbers.map((number) =>
         <li key={number.toString()}>
         {number}
         </li>
        );

The best way to pick a key is to use a string that uniquely identifies a list item among its siblings. Most often you would use IDs from your data as keys:

        const todoItems = todos.map((todo) =>
        <li key={todo.id}>
        {todo.text}
        </li>
        );

When you don’t have stable IDs for rendered items, you may use the item index as a key as a last resort:

        const todoItems = todos.map((todo, index) =>
        // Only do this if items have no stable IDs
        <li key={index}>
        {todo.text}
        </li>
        );

**Keys Must Only Be Unique Among Siblings**

# How to Use the Spread Operator (…) in JavaScript

The spread operator is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a function’s arguments.

## What is the spread operator?

In JavaScript, spread syntax refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.

> `“When ...arr is used in the function call, it ‘expands’ an iterable object arr into the list of arguments.”`

## What is ... used for?

> `“Spread operator to the rescue! It looks similar to rest parameters, also using ..., but does quite the opposite.”`

_Take trying to find the largest number in an array with Math.max():_

        Math.max(1,3,5) // 5
        Math.max([1,3,5]) // NaN

_Trying to pass an array to a JavaScript function expecting separate arguments does not work. In this case it produces a NaN result. Enter …:_

        Math.max(...[1,3,5]) // 5

_The spread syntax “spreads” the array into separate arguments._

## What else can … do?

The … spread operator is useful for many different routine tasks in JavaScript, including the following:

- Copying an array
- Concatenating or combining arrays
- Using Math functions
- Using an array as arguments
- Adding an item to a list
- Adding to state in React
- Combining objects
- Converting NodeList to an array

## Examples of using …

Here are a couple basic examples of using … in JavaScript, where I demonstrate copying an array, splitting a string into characters, and combining the properties of two JavaScript objects:

        [...["😋😛😜🤪😝"]] // Array [ "😋😛😜🤪😝" ]
        [..."🙂🙃😉😊😇🥰😍🤩!"] // Array(9) [ "🙂", "🙃", "😉", "😊", "😇", "🥰", "😍", "🤩", "!" ]

        const hello = {hello: "😋😛😜🤪😝"}
        const world = {world: "🙂🙃😉😊😇🥰😍🤩!"}

        const helloWorld = {...hello,...world}
        console.log(helloWorld) // Object { hello: "😋😛😜🤪😝", world: "🙂🙃😉😊😇🥰😍🤩!" }

### Copying an array

Using the … spread operator is a convenient way to copy an array or combine arrays, and it can even add new items:

        const fruits = ['🍏','🍊','🍌','🍉','🍍']
        const moreFruits = [...fruits];
        console.log(moreFruits) // Array(5) [ "🍏", "🍊", "🍌", "🍉", "🍍" ]
        fruits[0] = '🍑'
        console.log(...[...fruits,'...',...moreFruits]) //  🍑 🍊 🍌 🍉 🍍 ... 🍏 🍊 🍌 🍉 🍍

### Concatenating arrays

Asseen in the last example, the spread operator can quickly combine two arrays, an operation known as array concatenation:

        const myArray = [`🤪`,`🐻`,`🎌`]
        const yourArray = [`🙂`,`🤗`,`🤩`]
        const ourArray = [...myArray,...yourArray]
        console.log(...ourArray) // 🤪 🐻 🎌 🙂 🤗 🤩

### Adding an item to a list

Asnoted in the last example, the spread operator can add an item to an another array with a natural, easy-to-understand syntax:

        const fewFruit = ['🍏','🍊','🍌']
        const fewMoreFruit = ['🍉', '🍍', ...fewFruit]
        console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]

### Combining objects

The spread syntax is useful for combining the properties and methods on objects into a new object:

        const objectOne = {hello: "🤪"}
        const objectTwo = {world: "🐻"}
        const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}
        console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }
        const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("😂".repeat(5))}}
        objectFour.laugh() // 😂😂😂😂😂
