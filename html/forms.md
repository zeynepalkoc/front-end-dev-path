# Forms in HTML

Forms are used to collect user input.

Examples of form usage:

- login forms
- registration forms
- contact forms
- search bars

Forms are created using the `<form>` element.

---

# Basic Form Example

```html
<form>
  <label>Name:</label>
  <input type="text">

  <br><br>

  <label>Email:</label>
  <input type="email">

  <br><br>

  <button>Submit</button>
</form>
```
# İmportant Form Elements

From :

The <form> tag defines a form 

    Example:
    ```
<form>
</form>
```

# İnput
the <input> element allows users to enter data 

Example: 
```
<input type="text">
```

Common input types:
-text
-email
-password
-number
-date

Example:
```
<input type="password">
```

# Lable
labels describe input fields
```
<label>Email</label>
<input type="email">
```
labels improve accessibility and usability

# button
buttons are used to submit the form
```
<button>Submit</button>
```

# Example Forms

```
<h2>Contact Form</h2>

<form>

<label>Name</label>
<input type="text">

<br><br>

<label>Email</label>
<input type="email">

<br><br>

<label>Message</label>
<textarea></textarea>

<br><br>

<button>Send</button>

</form>
```

Common Beginner Mistakes

❌ Not connecting labels to inputs
❌ Using wrong input types
❌ Forgetting form structure
