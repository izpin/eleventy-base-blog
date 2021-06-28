---
title: The one about programing concepts.
description: This post is about learning the fundamentals of JavaScript.
date: 2018-05-01
tags:
  - basics tag
layout: layouts/post.njk
---
## The basics
We begin with a simple programme to calculate a bill total with tip.

<!-- is it poss to change the background colour? -->
```
const preTipTotal = 30.24;
const tip = preTipTotal * 0.15;

const total = preTipTotal + tip;
 
console.log("Your total bill, with a tip of £" + tip.toFixed(2) + ", is £" + total.toFixed(2) + ".");
```

<br/>

#### This short program includes:
1. Declaring const variables
1. Functional programming
1. Calling the write() and toFixed() methods
1. Concatenating a string

#### In the future I could expand this program to:
+ Accept input from the user
+ Calculate the change needed from a cash payment
+ Split the bill