# JavaScript Notes: Events

## **What are Events?**
Events are actions or occurrences that happen in the browser, such as a user clicking a button, typing on a keyboard, or moving the mouse. JavaScript can listen for these events and execute code in response.

---

## **Types of Events**

### **1. Mouse Events**
- **`click`**: Fired when an element is clicked.
- **`dblclick`**: Fired when an element is double-clicked.
- **`mouseover`**: Fired when the mouse pointer is over an element.
- **`mouseout`**: Fired when the mouse pointer leaves an element.
- **`mousemove`**: Fired when the mouse pointer is moving over an element.
- **`mousedown`**: Fired when a mouse button is pressed.
- **`mouseup`**: Fired when a mouse button is released.

### **2. Keyboard Events**
- **`keydown`**: Fired when a key is pressed.
- **`keyup`**: Fired when a key is released.
- **`keypress`**: Deprecated; use `keydown` or `keyup` instead.

### **3. Form Events**
- **`submit`**: Fired when a form is submitted.
- **`change`**: Fired when an input value changes.
- **`input`**: Fired when an input value is being entered.
- **`focus`**: Fired when an element gains focus.
- **`blur`**: Fired when an element loses focus.

### **4. Window Events**
- **`load`**: Fired when the entire page (including images and styles) has loaded.
- **`resize`**: Fired when the browser window is resized.
- **`scroll`**: Fired when the user scrolls the page.
- **`unload`**: Fired when the user navigates away from the page.

### **5. Touch Events (For Mobile)**
- **`touchstart`**: Fired when a touch point is placed on the screen.
- **`touchmove`**: Fired when a touch point is moved along the screen.
- **`touchend`**: Fired when a touch point is removed from the screen.

---

## **Adding Event Listeners**
JavaScript provides several ways to attach event listeners to elements.

### **1. Using HTML Attributes**
Attach an event directly in the HTML element.
#### Example:
```html
<button onclick="alert('Button clicked!')">Click Me</button>
```

### **2. Using `addEventListener`**
A modern and flexible way to add event listeners.
#### Syntax:
```javascript
element.addEventListener(event, function, options);
```
#### Example:
```javascript
const button = document.querySelector("button");
button.addEventListener("click", () => {
    console.log("Button clicked!");
});
```

### **3. Inline JavaScript (Not Recommended)**
Embedding JavaScript directly in HTML attributes is considered outdated.
#### Example:
```html
<button onclick="console.log('Inline JavaScript')">Click Me</button>
```

---

## **Event Object**
When an event is fired, an `Event` object is automatically passed to the event listener.

### **Properties of the Event Object**
- **`type`**: The type of event (e.g., `click`, `keydown`).
- **`target`**: The element that triggered the event.
- **`currentTarget`**: The element to which the event listener is attached.
- **`preventDefault()`**: Prevents the default action associated with the event.
- **`stopPropagation()`**: Stops the event from propagating further.

#### Example:
```javascript
const link = document.querySelector("a");
link.addEventListener("click", (event) => {
    event.preventDefault(); // Prevents the default action of opening the link
    console.log("Default action prevented");
});
```

---

## **Event Delegation**
A technique to handle events more efficiently by attaching a single event listener to a parent element.

### Why Use Event Delegation?
- Reduces the number of event listeners in the DOM.
- Handles dynamically added elements.

#### Example:
```javascript
const parent = document.querySelector("ul");
parent.addEventListener("click", (event) => {
    if (event.target.tagName === "LI") {
        console.log(`Clicked on: ${event.target.textContent}`);
    }
});
```

---

## **Common Use Cases**

### **1. Button Click**
#### Example:
```javascript
const button = document.querySelector("button");
button.addEventListener("click", () => {
    console.log("Button was clicked!");
});
```

### **2. Input Change**
#### Example:
```javascript
const input = document.querySelector("input");
input.addEventListener("input", (event) => {
    console.log(`Value: ${event.target.value}`);
});
```

### **3. Form Submission**
#### Example:
```javascript
const form = document.querySelector("form");
form.addEventListener("submit", (event) => {
    event.preventDefault(); // Prevent form from reloading the page
    console.log("Form submitted!");
});
```

### **4. Window Resize**
#### Example:
```javascript
window.addEventListener("resize", () => {
    console.log(`Window size: ${window.innerWidth} x ${window.innerHeight}`);
});
```

---

## **Best Practices**
1. Use `addEventListener` for flexibility and compatibility.
2. Avoid inline JavaScript for better maintainability.
3. Use `preventDefault` and `stopPropagation` carefully.
4. Use event delegation for better performance with many elements.
5. Clean up event listeners when they are no longer needed to prevent memory leaks.

#### Example of Cleaning Up:
```javascript
function handleClick() {
    console.log("Clicked!");
}

button.addEventListener("click", handleClick);
// Later...
button.removeEventListener("click", handleClick);
