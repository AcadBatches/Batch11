
# Pre-Assignment Notes: HTML Forms

---

## What are HTML Forms?
HTML Forms are a way to collect user input and send it to a server for processing. They are a core building block of web interactivity and are used for tasks like login, registration, search, and feedback collection.

---

## Key Elements of an HTML Form

### 1. `<form>` Tag
- Defines the beginning and end of a form.
- **Attributes**:
  - `action`: The URL where the form data is sent.
  - `method`: HTTP method for form submission (`GET` or `POST`).

```html
<form action="/submit" method="POST">
  <!-- Form Elements Here -->
</form>
```

---

### 2. Input Fields
- **`<input>`**: Collects user data.
  - `type` attribute defines the input type:
    - `text`, `password`, `email`, `number`, `date`, `checkbox`, `radio`, `file`, etc.

```html
<input type="text" name="username" placeholder="Enter your name">
```

---

### 3. Labels
- Use the `<label>` tag to associate a label with an input.
- Improves accessibility.

```html
<label for="username">Name:</label>
<input type="text" id="username" name="username">
```

---

### 4. Buttons
- **`<button>`** or `<input type="submit">`:
  - Submits the form.
- Can also use `<button type="button">` for custom functionality.

```html
<button type="submit">Submit</button>
```

---

### 5. Textarea
- Used for multi-line text input.

```html
<textarea name="comments" rows="4" cols="50"></textarea>
```

---

### 6. Select Dropdown
- Provides a dropdown list of options.

```html
<select name="options">
  <option value="option1">Option 1</option>
  <option value="option2">Option 2</option>
</select>
```

---

### 7. Radio Buttons and Checkboxes
- **Radio Buttons**: Select one option from a group.

```html
<input type="radio" name="gender" value="male"> Male
<input type="radio" name="gender" value="female"> Female
```

- **Checkboxes**: Select multiple options.

```html
<input type="checkbox" name="interests" value="coding"> Coding
<input type="checkbox" name="interests" value="reading"> Reading
```

---

### 8. Hidden Inputs
- Store data that is not visible to the user.

```html
<input type="hidden" name="token" value="12345">
```

---

## Form Validation

### 1. Client-side Validation
- Built-in attributes:
  - `required`: Makes a field mandatory.
  - `min`, `max`, `pattern`: Validates specific input criteria.

```html
<input type="email" name="email" required>
```

### 2. Server-side Validation
- Performed after form submission for security.

---

## Accessibility Tips
- Always use `<label>` tags for inputs.
- Use `aria-label` or `aria-describedby` for additional context.
- Provide clear error messages for invalid input.

---

## Example: Simple Login Form

```html
<form action="/login" method="POST">
  <label for="email">Email:</label>
  <input type="email" id="email" name="email" required>
  
  <label for="password">Password:</label>
  <input type="password" id="password" name="password" required>
  
  <button type="submit">Login</button>
</form>
```

---

## Assignment Tasks
1. Create a form for user registration with the following fields:
   - Name, email, password, gender (radio), and hobbies (checkbox).
   - Include proper labels and validation.
2. Style the form using basic CSS to make it user-friendly.
3. Test the form to ensure validation works correctly for different input types.
