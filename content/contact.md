---
title: Contact
layout: default
tags: [primary, footer]
---

<form>
  <p><strong>This is just a test form. It doesn't do anything.</strong></p>
  <p>
  <select>
	<option selected="selected" value="1">Title</option>
	<option value="2">Mr</option>
    <option value="3">Miss</option>
    <option value="4">Mrs</option>
    <option value="5">Other</option>
	</select>
  </p>
  <p>
  <label>First name</label>
  <input type="text" name="first_name" />
  </p>
  <p>
  <label>Surname</label>
  <input type="text" name="surname" />
  </p>
  <p>
  <label>Email</label>
  <input type="email" name="email" required="" />
  </p>
  <p>
  <label>Enquiry type:</label>
  <label><input checked="checked" name="type" type="radio" value="sales" /> Sales</label> 
  <label><input name="type" type="radio" value="support" /> Support</label> 
  <label><input name="type" type="radio" value="billing" /> Billing</label>
  </p>
  <p>
  <label>
  <input type="checkbox" id="checkbox" value="terms" />
  I agree to the <a href="#">terms and conditions</a>
  </label>
  </p>

<button>Send</button>
<button type="reset">Reset</button>
<button disabled="disabled">Disabled</button>

</form>
