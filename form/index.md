---
layout: layouts/post.njk
title: Contact Form
templateClass: tmpl-post
eleventyNavigation:
  key: Form
  order: 7
---
<br>

<div id=form-body>
<form name="submitted" method="POST" data-netlify="true" netlify-honeypot="bot-field">

<p class="hidden">
    <label>Don’t fill this out if you’re human: <input name="bot-field" /></label>
  </p>

  <div class=form-group>
    <label for="firstname">First name</label>
    <div class=input-group>
      <input type="text" name="firstname" id="firstname" class="inputstyle"  required/>
    </div>
  </div>

  <div class=form-group>
    <label for="surname">Surname</label>
    <input type="text" name="surname" id="surname" class="inputstyle" required/>
  </div>

  <div class=form-group>
    <label for="Email">Email</label>
    <input type="email" name="email" id="Email" class="inputstyle" required/>
  </div>

  <div class=form-group>
    <label for="Message">Your message</label>
    <div>
        <textarea id="Message" name="Message"  rows="6" maxlength="3000" class="inputstyle" required></textarea>
    </div> 
  </div>

  <div class="submit-btn">
  <input type="submit" value="Submit" >
  </div>
  
</form>

</div>

