---
layout: layouts/post.njk
title: Contact Form
templateClass: tmpl-post
eleventyNavigation:
  key: Contact
  order: 7
---
<br>

<div id=form-body>
<form name="submitted" method="POST" data-netlify="true" netlify-honeypot="bot-field">

<p class="hidden">
    <label>Don’t fill this out if you’re human: <input name="bot-field" /></label>
  </p>

  <div class="row form-group">
  <div class="col input-group">
    <input type="text" name="firstname" id="firstname" class="form-control inputstyle" placeholder="First name" aria-label="First name" aria-required="true" required>
  </div>
  <div class="col input-group">
    <input type="text" name="surname" id="surname" class="form-control inputstyle" placeholder="Last name" aria-label="Last name" aria-required="true" required>
  </div>
</div>

<div class="row form-group">
  <div class="col input-group">
    <input type="email" name="email" id="Email" class="form-control inputstyle" placeholder="Email" aria-label="Email" aria-required="true" required>
  </div>
</div>

<div class="row form-group">
  <div>
        <textarea id="message" name="message"  rows="6" maxlength="3000" class="form-control inputstyle" placeholder="Message" aria-label="Message" aria-required="true" required></textarea>
    </div>
</div>

  <div class="submit-btn">
  <input type="submit" class="btn btn-light" value="Submit" >
  </div>
  
</form>

</div>

