<!-- ---
layout: layouts/post.njk
title: Photo filter
templateClass: tmpl-post
eleventyNavigation:
  key: Photo filter Project
  order: 4
--- -->

## A second project using the DOM with JavaScript.

This project has a prebuilt selection of images. The user can filter these images using form elements. This is done by searching the alt tags using the search box e.g. ‘smile’, or by selecting a button labeled by animal or ‘show all’ to reset the images. The page works by adding the class 'hidden' to the elements we want to hide - i.e the elements that don't match the search terms.

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

1. Accepts input from the user to trigger filter behaviour using event listeners.
1. Accesses the DOM by id, class name and querySelector to get information about the form and the images.
1. A 'click' event listener establishes what button/animal as selected.
   - The 'getAttribute' method retrieves custom attribute data for "animal".
   - A for loop iterates through all the images.
     - Control flow 'if' statements, logical operators and strict comparison to determine which images match the button filter.
1. When the user types, a 'keyup' event listener takes the characters typed in the search bar and stores it in a variable.
   - this variable is converted into a regular expression.
   - we loop through all the images.
   - In an if statement we append the method test() to the regular expression and pass in the image's alt tag (which has also been stored in a new variable) to determine if the alt tag matches the image.
1. If there's a match in either if/ corresponding else statement, the class list is updated, using CSS class styling to alter the state of images. The class "hidden" is removed from the particular image if the if statement evaluates to true. This ensures the image is visible. Else the class "hidden" is added in order to hide the image.

**Improvements to add:**

- Take into account the selected filter button – so the input text ‘smile’ and selecting ‘dog’ will only show images of smiling dogs. Instead of only using one filtering method at a time.
- Add responsive styling to centre the images, resize them or change the number in a row given the size of the user’s window.
- Add CSS classes that show which filter is currently selected.
  - This could be achieved by adding a border to the clickable element.
- Add helper text above the images such as “showing animals that match the search “{searchString}” and the filter {filter}".
