---
title: The one about loops, arrays and objects
description: This post is about learning to use loops, arrays and objects in JavaScript.
date: 2021-05-17
tags: fifth tag
layout: layouts/post.njk
---

## The basics

```
var recipe = {
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

#### This short program includes:
1. For loops and interating
1. Arrays
1. Objects
1.  

#### In the future I could expand this program to:
+ 
+ 
+ 

## The basics

working with data that has been provided to us

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
```

<a href="{{ '/posts/fourthpost/' | url }}">Fourth post</a>