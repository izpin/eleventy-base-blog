---
layout: layouts/post.njk
title: To-Do List
templateClass: tmpl-post
eleventyNavigation:
  key: To-Do List Project
  order: 3
---

### My first project using JavaScript and the Document Object Model (DOM)!
<br>

**Defined by [MDN](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction) as** <em>“the data representation of the objects that comprise the structure and content of a document on the web.”</em>

**The DOM is** <em> “a programming interface for HTML and XML documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects."</em>

This allows programming and scripting languages to connect to and change a web page.

We can write in JavaScript (or another language such as Python) in order to use the DOM to access and dynamically manipulate elements and documents. 

## The To-Do list project

This project should create a list of current to-dos for a user. It accepts text data to form the content of the list item as well as a priority indicating the urgency of the task. The list builds top to bottom, with the latest added to the bottom. The most recent to-do is the only item with the class 'just-created'.

Project before user input.

<a href="https://codepen.io/izpin/details/gOWOLba">
  <img src="/img/tdl.png" class="codepen" alt="To-do list project without to-dos">
</a>

To-do list with to-dos added. Currently, the list doesn't display information about the priority selected.

<a href="https://codepen.io/izpin/details/gOWOLba">
  <img src="/img/tdl-withtds.png" class="codepen" alt="To-do list project with to-dos added">
</a>

This code-pen project accepts input from the user in the form of text (the specific task) and a dropdown box (the priority of the task). This is then translated into a to-do list using event listeners and selectors. 

**Components of my JavaScript code using the DOM:**

1. Selectors to get individual elements.
1. Selectors to get a live list – a list that is dynamic and updates automatically as we add to-dos.
1. Event listeners	-submit	- use parameter even to use preventDefault() to stop the submit to server behaviour.
1. Method reset() to clear the form for the next to-do.
1. For loops to remove/add the class ‘just-created’ to the most recent to do.	
    + I have used console.log to test and debug in conjunction with the live list.
1. Create new nodes in order to append to child nodes to parent elements and insert them into the DOM – ie to actually create the new to-do.

**Features to add:**
+ Integrate the priority option value - to be illustrated using a combination of images and colour-coding.

<img src="https://cdn1.iconfinder.com/data/icons/prettyoffice8/256/Flag-green.png" class="flag" alt="Green flag, low priority">
<img src="https://cdn1.iconfinder.com/data/icons/prettyoffice8/256/Flag-yellow.png" class="flag" alt="Yello flag, medium priority">
<img src="https://cdn1.iconfinder.com/data/icons/prettyoffice8/256/Flag-red.png" class="flag" alt="Red flag, high priority">

+ Add functionality that deletes to-dos as they’re completed
	+ Could do this with a 'click' event listener.
