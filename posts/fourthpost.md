---
title: The one about pseudocode
description: This post is about learning to use pseudocode.
date: 2021-05-17
tags: pseudocode
layout: layouts/post.njk
---

## The basics

### Pseudo - Something that is like something else

Pseudocode allows a programmer to focus on the logic of solving a problem rather than becoming bogged down with the semantics and syntax immediately. Eventually, through implementation, this produces a program.

Or, put another way, it is a method of abstraction used to make creating an algorithm more approachable.

##### For example, we might have a brief like this:
Keep track of which books you read and which books you want to read!

Create an array of objects, where each object describes a book and has properties for the title (a string), author (a string), and already read (a boolean indicating if you read it yet).

Iterate through the array of books. For each book, log the book title and book author like so: “The Hobbit by J.R.R. Tolkien”.

Now use an if/else statement to change the output depending on whether you read it yet or not. If you read it, log a string like ‘You already read “The Hobbit” by J.R.R. Tolkien’, and if not, log a string like ‘You still need to read “The Lord of the Rings” by J.R.R. Tolkien.’

##### The pseudocode might read like this:
```
CREATE array of objects, books, w/ 3 properties
					{	title: ‘string’;
						author: ‘string’;
						alreadyRead: bool;
					}
LOOP through array, for each book
	PRINT title + author in the format “Title by Author”
	
	IF	alreadyRead === true
		PRINT ‘You already read “Title by Author" ‘
	ELSE 	
    PRINT ‘You still need to read “Title by Author” ‘ 
```


**Note that we have:**
1. Used mostly brief, human-like language rather than a programming specific language
1. Capitalised syntax such as <em>if, else</em> to help when it comes to actually implementing the program.
1. Used indentation to make it more readable and to show where elements are nested.

   
<a href="{{ '/posts/thirdpost/' | url }}">Third post</a>
<a href="{{ '/posts/fifthpost/' | url }}">Fifth post</a>
