---
layout: layouts/post.njk
title: Form
templateClass: tmpl-post
eleventyNavigation:
  key: Form
  order: 7
---
<br>
<form name="submitted" method="POST" data-netlify="true">
  <label for="Username">Username</label>
  <input type="text" name="username" id="Username"/>
  <br>
  <label for="Email">Email</label>
  <input type="email" name="email" id="Email"/>
  <br>
  <label for="Password">Password</label>
  <input type="password" name="password" id="Password"/>
  <br>
  <label for="PhoneNumber">Phone Number</label>
  <input type="tel" id="PhoneNumber" name="phoneNumber"/>
  <br>
  <label for="date">Date of Purchase</label>
  <input type="date" id="date" name="date"/>
  <br>
  
  <fieldset>
    <legend>Mailing list</legend>
  <label for="list">News</label>
    <input type="checkbox" id="list" name="list"/>
  <label for="list">Offers</label>
    <input type="checkbox" id="list" name="list"/>
  </fieldset>
  <br>
  
  <label for="starSign"> Your star sign: </label>
  <select id="starSign">
    <optgroup label="Fire sign:">
      <option> Aries </option>
      <option> Leo </option>
      <option> Sagittarius </option>
    </optgroup>
    <optgroup label="Earth sign:">
      <option> Taurus </option>
      <option> Virgo </option>
      <option> Capricorn </option>
    </optgroup>
    <optgroup label="Air sign:">
      <option> Gemini </option>
      <option> Libra </option>
      <option> Aquarius </option>
    </optgroup>
    <optgroup label="Water sign:">
      <option> Cancer </option>
      <option> Scorpio </option>
      <option> Pisces </option>
    </optgroup>
  <br>
  <p><input type="submit" value="Submit"></p>
</form>