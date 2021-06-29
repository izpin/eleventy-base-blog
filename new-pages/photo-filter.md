---
layout: layouts/post.njk
title: Photo filter
templateClass: tmpl-post
eleventyNavigation:
  key: Photo filter Project
  order: 4
---

### My second project using the DOM via JavaScript.

This project has a prebuilt selection of images. The user can filter these images either by searching the alt tags with the search box – e.g. ‘smile’ or by the predefined buttons by animal or ‘show all’ to reset the images. The page works by adding the class 'hidden' to the elements we want to hide - i.e the elements that don't match the search terms.

<!-- [![Animal photo filter project with all images showing](/img/afilter-all.png)](https://codepen.io/izpin/full/ZEedMza) -->

With all images showing - no filters applied:

<a href="https://codepen.io/izpin/full/ZEedMza">
  <img src="/img/afilter-all.png" class="codepen" alt="Animal photo filter project with all images showing">
</a>

Images with animal attribute 'dog' showing - selected using the buttons:

<a href="https://codepen.io/izpin/full/ZEedMza">
  <img src="/img/afilter-dog.png" class="codepen" alt="Animal photo filter project with images with animal attribute 'dog' showing">
</a>

Showing images with alt tag 'water' showing, taken from user inputted text in the search box:

<a href="https://codepen.io/izpin/full/ZEedMza">
  <img src="/img/afilter-water1.png" class="codepen" alt="Animal photo filter project with images with alt tag 'water' showing">
</a>


**Current features of Animal Filter:**
1. Accepting input from the user to trigger events using the event listener for ‘click’.
1. Accessing the DOM by id, class name and querySelector.
1. Use of 'getAttribute' method to retrieve custom attribute data for "animal".
1. Multiple 'for of' loops to iterate through these elements.
1. Control flow 'if' statements and logical operators to determine if these are the correct images.
1. Updating class list and using CSS styling to change the state of images – change between hidden and visible depending on the filters used.


**Improvements to add:**

+ Take into account the selected filter button – so the input text ‘smile’ and selecting ‘dog’ will only show images of smiling dogs. Instead of only using one filtering method at a time.

+ Add responsive styling to centre the images, resize them or change the number in a row given the size of the user’s window.

+ Add CSS classes that show which filter is currently selected 
  + can achieve this by adding a border to the clickable element.

+ Add helper text above the images such as “showing animals that match the search “{searchString}” and the filter {filter}".



