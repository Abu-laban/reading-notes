# Review, Research, and Discussion

---

## Describe (in plain English) what Array.map() does

**Array.map()**

> Array.Map() is used to create a new array by calling a function on each element of the passed array, **in order**.

* Note: this method does not change the original array.

---

## Describe (in plain English) what Array.reduce() does

**Array.reduce()**

> Reduce is a well named method. It takes an array and reduces it to a single value.( or fold, or accumulate )

It takes a function as its first parameter. This function can take 4 arguments. It can also take a optional second argument, which is the initial value to the first call of the function. Like so :

``[0, 1, 2, 3].reduce( function( accumulator, currentValue, currentIndex, array ){}, [ initialValue ])``

*The accumulator receives the value returned by the callback function after each iteration. It accumulates it to the previous value it had.*

*The currentValue is the current value being processed in the array. The currentIndex is the current index being processed in the array. array is the target array reduce is called on.*

> The initialValue is an optional value that indicates if the first value should be different than the first index of the array. If you supply this, reduce will start at index 1 in the array.

---

## Provide code snippets showing how to use superagent() to fetch data from a URL and log the result

- With normal Promise .then() syntax

![async_await](async_await.PNG)


- Again with async / await syntax


![then](then.PNG)

---

## Explain promises as though you were mentoring a Code 301 level student

A **promise** is an object that encapsulates the result of an ``asynchronous operation``.

---

## Are all callback functions considered to be Asynchronous? Why or Why Not?

Well, basically yes, but there's a catch. Every asynchronous function takes a function argument, but not every function that does so is asynchronous. It matters how the argument is used inside the function.

> Simply taking a callback doesn't make a function asynchronous. There are many examples of functions that take a function argument but are not asynchronous. For example there's forEach in Array. It iterates over each item and calls the function once per item.