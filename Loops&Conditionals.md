# JavaScript Notes: Conditions & Loops

## **Conditions**
Conditions are used to execute code based on specific criteria.

### **1. `if` Statement**
Executes a block of code if a specified condition is true.

#### Syntax:
```javascript
if (condition) {
    // Code to execute if condition is true
}
```
#### Example:
```javascript
let age = 18;
if (age >= 18) {
    console.log("You are an adult.");
}
```

### **2. `if-else` Statement**
Executes one block of code if the condition is true, otherwise executes another block.

#### Syntax:
```javascript
if (condition) {
    // Code to execute if condition is true
} else {
    // Code to execute if condition is false
}
```
#### Example:
```javascript
let age = 16;
if (age >= 18) {
    console.log("You are an adult.");
} else {
    console.log("You are a minor.");
}
```

### **3. `if-else if-else` Statement**
Allows multiple conditions to be checked in sequence.

#### Syntax:
```javascript
if (condition1) {
    // Code if condition1 is true
} else if (condition2) {
    // Code if condition2 is true
} else {
    // Code if all conditions are false
}
```
#### Example:
```javascript
let score = 85;
if (score >= 90) {
    console.log("Grade: A");
} else if (score >= 75) {
    console.log("Grade: B");
} else {
    console.log("Grade: C");
}
```

### **4. `switch` Statement**
Tests a variable against multiple cases and executes the matching block of code.

#### Syntax:
```javascript
switch (expression) {
    case value1:
        // Code to execute if expression === value1
        break;
    case value2:
        // Code to execute if expression === value2
        break;
    default:
        // Code to execute if no case matches
}
```
#### Example:
```javascript
let day = 3;
switch (day) {
    case 1:
        console.log("Monday");
        break;
    case 2:
        console.log("Tuesday");
        break;
    case 3:
        console.log("Wednesday");
        break;
    default:
        console.log("Invalid day");
}
```

---

## **Loops**
Loops are used to execute a block of code repeatedly.

### **1. `for` Loop**
Loops through a block of code a specific number of times.

#### Syntax:
```javascript
for (initialization; condition; increment) {
    // Code to execute
}
```
#### Example:
```javascript
for (let i = 0; i < 5; i++) {
    console.log(i);
}
```

### **2. `while` Loop**
Executes a block of code as long as the specified condition is true.

#### Syntax:
```javascript
while (condition) {
    // Code to execute
}
```
#### Example:
```javascript
let i = 0;
while (i < 5) {
    console.log(i);
    i++;
}
```

### **3. `do-while` Loop**
Executes a block of code once, then repeats as long as the condition is true.

#### Syntax:
```javascript
do {
    // Code to execute
} while (condition);
```
#### Example:
```javascript
let i = 0;
do {
    console.log(i);
    i++;
} while (i < 5);
```

### **4. `for...in` Loop**
Loops through the properties of an object.

#### Syntax:
```javascript
for (key in object) {
    // Code to execute
}
```
#### Example:
```javascript
let person = { name: "Alice", age: 25 };
for (let key in person) {
    console.log(key + ": " + person[key]);
}
```

### **5. `for...of` Loop**
Loops through the values of an iterable object (e.g., array).

#### Syntax:
```javascript
for (value of iterable) {
    // Code to execute
}
```
#### Example:
```javascript
let colors = ["red", "green", "blue"];
for (let color of colors) {
    console.log(color);
}
