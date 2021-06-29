---
title: The one about loops, arrays and objects
description: This post is about learning to use loops, arrays and objects in JavaScript.
date: 2021-05-17
tags: loops arrays objects
layout: layouts/post.njk
---

## A basic introduction

**Loops** ["help in executing one or more statements up to a desired number of times"](https://www.tutorialspoint.com/computer_programming/computer_programming_loops.htm). They evaluate statements against conditions, which will execute certain lines of code while they evaluate to true. They will execute until a statement (which is updated - eg. increased or decreased - following 1 loop or execution of the code within the loop) evaluates to false. 
  + Types of loops include:
    + While
    + Do while
    + For
    + For of (used in Javascript to iterate over iterable objects like arrays)

**Arrays** are ["a collection of items stored at contiguous memory locations"](https://www.geeksforgeeks.org/introduction-to-arrays/) - i.e consecutive blocks are used to store the data. This means we can access the information stored in the array using <em> indexing </em>
  + Arrays use zero-based indexing where the first value is stored at 0, so the last element is always stored at [lengthOfArray - 1].
    + So, we access the 1st item of an array using arr[0] the 2nd with arr[1] and so on.

Arrays are ["container-like values that can hold other values. The values inside an array are called elements."](https://www.javascript.com/learn/arrays) In JavaScript arrays can store multiple different types of data. So we can store whole numbers (integers) next to strings, next to bools.
  + we might initialise an array like this where the values are enclosed in square brackets and values are comma-seperated:
    + const arr = [3, "hello", "world", 4.56];


**Objects** ["Objects are variables too. But objects can contain many values... The values are written as name:value pairs (name and value separated by a colon)."](https://www.w3schools.com/js/js_objects.asp)
  + arrays are a type of object.  

Below we have created an object called recipe which contains the afforemention name:value (or key:value) pairs. We can also see we can store any datatype, including arrays, within an object: 
```
const recipe = {
  title: 'fried eggs',
  servings: 2,
  ingredients: ["eggs", "oil", "salt", "pepper"],
  directions: ["Heat oil in frying pan", "crack egg into pan", "cook until desired runiness", "season", "serve"]
};

function letsCook(recipe) {
  console.log(`I'm hungry! Let's cook ${recipe.title}.`)
  console.log(`${recipe.title} (for ${recipe.servings})`);
  console.log('Ingredients:');

  for (const ingredient of recipe.ingredients){
    console.log(`-${ingredient}`);
  }

  console.log('Directions:');

  for (const direction of recipe.directions){
    console.log(`-${direction}`);
  }
}

letsCook(recipe);
```

##### The above program:
1. Declares and initialises an object called recipes which includes values that are inetegers, strings and arrays,
1. A function called letsCook is declared, which we can pass the object into as a parameter. 
1. Multiple strings are printed using console.log and template literals. Dot notation is used to acess the value stored inside the object. e.g recipe.title will print the string 'fried eggs'.
1. A <em>for of</em> loop is used to access the data stored inside the array value at recipe.ingredients. This loop iterates through each value in the array and logs it to the console.
    + the loop declares a variable const ingredient for each element at recipe.ingredient, so it loops through the array the correct number of times and prints all the ingredient strings.
1. This is same principle is used to print the strings stored in the array recipe.direction.
1. We don't need to return any strings as we've been logging them as the function is executed and we don't meed to use them outside of the function.
1. The function is called in the last line of the program.

##### In the future I could expand this program to:
+ Store multiple recipe objects inside the variable recipe

<!-- working with data that has been provided to us

```
let shoppingCart = [
  { name: "loaf of bread", type: "food", quantity: 1, price: 0.85 },
  { name: "multipack beans", type: "food", quantity: 1, price: 1 },
  { name: "mushrooms", type: "food", quantity: 10, price: 0.1 },
  { name: "can of beer", type: "alcohol", quantity: 4, price: 1.1 },
  { name: "prosecco", type: "alcohol", quantity: 1, price: 8.99 },
  { name: "steak", type: "food", quantity: 2, price: 3.99 },
  { name: "blue cheese", type: "food", quantity: 1, price: 2.99 },
  { name: "candles", type: "home", quantity: 3, price: 1.99 },
  { name: "cheesecake", type: "food", quantity: 1, price: 4.99 },
  { name: "onions", type: "food", quantity: 3, price: 0.4 },
];

//function to create an array of items within a specific budget

function filterCart(cart, lowPrice, highPrice, quantity) {
  const items = [];

    for (const item of cart){
      if (quantity === true && item.price * item.quantity >= lowPrice && item.price * item.quantity <= highPrice) {
        items.push(item);
      }
      
      if (quantity === false && item.price >= lowPrice && item.price <= highPrice) {
        items.push(item);
      }
    }
    return items;
  }

console.log(filterCart(shoppingCart, 0.5, 2, true));
```

#### This short program includes:
1. Using for loops to iterate through data to 
1. Logical operators
1. Arrays
1. Objects
1. Pre-written JS methods e.g. .push()
1. Bool data type

```
//calculate shopping bill total, including discounts
function total(cart, discountAmount, type) {
    let totalPrice = 0;

    for (const item of cart){
      totalPrice += item.price * item.quantity;
      console.log(totalPrice);

      if (item.type === type || type === 'any') {
        const discount = (item.price * item.quantity) * discountAmount / 100;
        totalPrice -= discount;
      }
    }
    return totalPrice;
  }

console.log(total(shoppingCart, 20, 'any'));
``` -->

<a href="{{ '/posts/fourthpost/' | url }}">Fourth post</a>