---
title: The one about functions and control flow
description: This is a post on writing functions and some control flow in JavaScript.
date: 2018-07-04
tags:
  - control flow
layout: layouts/post.njk
---


## Should I wear a coat?
There's nothing worse than thinking you should've brought your big coat out with you. Let's create a program to solve this!

Brit-pick warning: beware the farenheit!

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

##### This program:
1. Declares a const variable - an int that represents a temperature.
1. Applies arbitrary logic to the variable to decide if we need a coat.
    + Conditional statements are never set in stone and we continue to update them if they fail to meet our logical needs. What I consider shorts and a tshirt weather might be someone elses big coat weather. 
      + Uni Izzy wouldn't take a coat out no matter the temperature - nights out in Newcastle in the sleet and snow wearing jeans and a nice top? Completed it. Frost bite? Don't know her. 
1. Uses control flow: <em>if, else if</em> and <em>else</em> statements decide which lines of code to execute given a condition.
1. The <em>logical operator '&&'</em>, is used where two <em>boolean expressions</em> must be true in order for a statement to execute -ie temp is greater or equal to one number, but lower than or equal to another.
1. When a statement is evaluated to 'true' the code inside the following curly braces is executed. In this program it is always a log() to the console that communicates an outcome to the user.

##### In the future I could expand this program to:
+ Accept input from the user
+ Convert from celcius to farenheit + vice versa
+ 

<a href="{{ '/posts/firstpost/' | url }}">First post</a>
<a href="{{ '/posts/thirdpost/' | url }}">Third post</a>

