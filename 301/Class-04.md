# React and Forms

# Forms

HTML form elements work a bit differently from other DOM elements in React, because form elements naturally keep some internal state.

## Controlled Components

n HTML, form elements such as `<input>`, `<textarea>`, and `<select>` typically maintain their own state and update it based on user input. In React, mutable state is typically kept in the state property of components, and only updated with setState().

We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a **“controlled component”**.

> should we update the state with their responses as soon as they enter them.

Since the value attribute is set on our form element, the displayed value will always be this.state.value, making the React state the source of truth. Since handleChange runs on every keystroke to update the React state, the displayed value will update as the user types.

## With a controlled component, the input’s value is always driven by the React state. While this means you have to type a bit more code, you can now pass the value to other UI elements too, or reset it from other event handlers.

# The Conditional (Ternary) Operator

Using a conditional, like an `if` statement, allows us to specify that a certain block of code should be executed _if_ a certain condition is met.

## The ternary operator:

just one line of code

> **condition ? value if true : value if false**

### Here’s what you need to know:

1. The `condition` is what you’re actually testing. The result of your condition should be `true` or `false` or at least coerce to either boolean value.

2. A `?` separates our conditional from our **true** value. Anything between the `?` and the `:` is what is executed if the `condition` evaluates to **true**.

3. Finally a `:` colon. If your `condition` evaluates to **false**, any code after the colon is executed.

\_ _Rewrite the following statement using a ternary_

        statement:
        if(x===y){
        console.log(true);
        } else {
         console.log(false);
         }

> x === y ? console.log(true) : console.log(false) ;

![flash](img/ternary.PNG)
