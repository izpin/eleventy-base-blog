---
title: The one about functions and control flow
description: This is a post on writing functions and some control flow in JavaScript.
date: 2018-07-04
tags:
  - control flow
layout: layouts/post.njk
---


## Shall I wear a coat?
There's nothing worse than thinking you should've brought your big coat out with you. Let's create a program to solve this!

Brit warning: beware the farenheit

```
const temp = 30;

if(temp < 0){
  console.log('stay inside');
}
else if(temp >= 0 && temp < 30){
  console.log('wear a coat and hat');
}
else if(temp >= 30 && temp < 50){
  console.log('wear a coat');
}
else {
   console.log('just pants and vest is fine');
}
```

#### This short program includes:
1. Declaring const variables
1. Functional programming.
1. Control flow: if, else if and else statements to decide which lines of code to execute given a condition.
1. The logical operator '&&', where two conditions must be met in order for a conditition to execute.

#### In the future I could expand this program to:
+ Accept input from the user
+ Convert from celcius to farenheit + vice versa
+ 

<a href="{{ '/posts/firstpost/' | url }}">First post</a>
<a href="{{ '/posts/thirdpost/' | url }}">Third post</a>

