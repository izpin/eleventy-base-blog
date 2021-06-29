---
title: The one about programing concepts.
description: This post is about learning the fundamentals of JavaScript.
date: 2018-05-01
tags:
  - basics
layout: layouts/post.njk
---
## The basics
We begin with a simple programme to **calculate a bill total with tip**.

This program is written in **JavaScript**. While ["initially created to 'make web pages alive'"](https://javascript.info/intro) and is the ["most widely-adopted browser language with full integration in HTML/CSS"](https://javascript.info/intro), for the purpose of this blog post, it is simply used to demonstrate some basic programming concepts.

<!-- is it poss to change the background colour? -->
```
const preTipTotal = 30.24;
const tip = preTipTotal * 0.15;

const total = preTipTotal + tip;
 
console.log("Your total bill, with a tip of £" + tip.toFixed(2) + ", is £" + total.toFixed(2) + ".");
```

<br/>

##### This short program:
1. Declares a const variable, i.e a variable that can't be changed accidentally as it can't be updated or re-declared.
    + Note the use of camelCasing when naming variables to clearly communicated what data they store. 
1. Applies a maths calculation to the previously declared variable and immediately initalises this (or stores this data) to a new const variable to hold the output of the calculation.
1. Rinse and repeat.
1. Calls the log() and toFixed() methods to print a string to the browser console and display to the variable 'total' rounded to 2 decimal places so the user can actually read the data stored in the variables. 
    + The string printed is <em>concatenated</em> - it joins character strings 'end-to-end' or immediately after each other exactly as they are stored. Note: therefore be careful to add your own white space/punctuation to your strings - its won't put spacing between words in a sentence for you.

##### In the future I could expand this program to:
+ Accept input from the user - make the code dynamic rather than static and hard coded.
+ Calculate the change needed from a cash payment.
+ Add functionality to be able to split the bill.