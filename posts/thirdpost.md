---
title: The one about switch statements.
description: This is a post about switch statements.
date: 2018-08-24
tags:
  - switch
layout: layouts/post.njk
---


## Section Header

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

#### This short program includes:
1. Variables with global and local scope.
1. Creating functions, passing arguments, applying logical code to these arguments in order to return a statement.
1. Template literals to print
1.  Switch statements

#### In the future I could expand this program to:
+ Accept input from the user
+ 
+ 

<a href="{{ '/posts/secondpost/' | url }}">Second post</a>
<a href="{{ '/posts/fourthpost/' | url }}">Fourth post</a>