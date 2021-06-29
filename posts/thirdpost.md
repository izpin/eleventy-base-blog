---
title: The one about switch statements.
description: This is a post about switch statements.
date: 2018-08-24
tags:
  - switch
layout: layouts/post.njk
---


## Let's get drinks! From the vending machine

This short program confirms with a user what drink they have ordered.

```
function drinkOrder(size, drink) {
  switch(drink) {
    case 'orange':
        softDrinkLabel = 'Orangeade';
        break;
      case 'lemon':
        softDrinkLabel = 'Lemonade';
        break;
      case 'cola':
        softDrinkLabel = 'Cola';
        break;
  }
  return `You have ordered a ${size} ${softDrinkLabel}.`;
}

const myOrder = drinkOrder('medium', 'lemon')
console.log(myOrder); 
```

##### This program:
1. Declares the function drinkOrder which accepts 2 parameters - size and drink. In JavaScript we don't have to declare that data types of variables or parameters. 
1. Variables declared outside have global scope, while the  variables in the function have local scope - they can't be referred to outside of the function. 
1. Inside the function we apply logic to the code using a switch statement which uses cases.
    + the logic here says: if the drink is 'orange' store the value 'Orangeade' in the variable softDrinkLabel then break out of the statement, else continue to the next case.
1. Once to switch statment breaks, a string is returned. Instead of concatenating a string, we have use <em>template literals</em> create a string. This uses single back ticks `` instead of quotation marks and the format ${variable} to pass a variables into the string.
1. We have stored this string in a variable myOrder by simultaneously initialising the variable and calling the function with our parameters/arguments passed in on the right and assigning the returned string to the variable on the left.
1. We then use console.log() to display the string stored in the variable. 

##### In the future I could expand this program to:
+ Accept input from the user
+ Add a default case for if the order doesn't match any available drinks

<a href="{{ '/posts/secondpost/' | url }}">Second post</a>
<a href="{{ '/posts/fourthpost/' | url }}">Fourth post</a>