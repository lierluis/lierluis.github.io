---
layout: page
title: Contact
permalink: /contact/
---

<form method="POST" action="https://formspree.io/luis.es@yahoo.com">

  <!-- FROM -->
  <div class="field is-horizontal">
    <div class="field-label is-normal">
      <label class="label">From</label>
    </div>
    <div class="field-body">
      <div class="field is-grouped">
        <p class="control is-expanded has-icons-left">
          <input class="input" type="text" name="name" placeholder="Name">
          <span class="icon is-small is-left">
            <i class="fa fa-user"></i>
          </span>
        </p>
      </div>
      <div class="field">
        <p class="control is-expanded has-icons-left">
          <input class="input" type="email" name="email" placeholder="Email">
          <span class="icon is-small is-left">
            <i class="fa fa-envelope"></i>
          </span>
        </p>
      </div>
    </div>
  </div>

  <!-- MESSAGE -->
  <div class="field is-horizontal">
    <div class="field-label is-normal">
      <label class="label">Message</label>
    </div>
    <div class="field-body">
      <div class="field">
        <div class="control">
          <textarea class="textarea" name="message" placeholder="Message"></textarea>
        </div>
      </div>
    </div>
  </div>

  <!-- SPAM -->
  <input type="text" name="_gotcha" style="display:none" />

  <!-- SEND -->
  <div class="field is-horizontal">
    <div class="field-label">
      <!-- Left empty for spacing -->
    </div>
    <div class="field-body">
      <div class="field">
        <div class="control">
          <input class="button is-primary" type="submit" value="Send">
        </div>
      </div>
    </div>
  </div>

</form>
