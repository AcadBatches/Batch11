# JavaScript Notes: Variables & Data Types, Operators

## **Variables**
Variables are used to store data values in JavaScript. 

### **Declaring Variables**
1. **`var`**: Global or function-scoped.
2. **`let`**: Block-scoped, allows reassignment.
3. **`const`**: Block-scoped, used for constants (cannot be reassigned).

#### **Syntax**:
```javascript
var x = 5;      // Global/function-scoped
let y = 10;     // Block-scoped
const z = 15;   // Block-scoped, constant
```

---

## **Data Types**

### **Primitive Data Types**
1. **Number**: Numeric values (e.g., `42`, `3.14`).
2. **String**: Textual data (e.g., `"hello"`, `'world'`).
3. **Boolean**: Logical values (`true` or `false`).
4. **Undefined**: A variable declared but not assigned a value.
5. **Null**: Represents an intentional absence of any object value.
6. **Symbol**: A unique and immutable data type (introduced in ES6).
7. **BigInt**: For very large integers (introduced in ES2020).

#### **Example**:
```javascript
let num = 42;           // Number
let name = "Alice";     // String
let isActive = true;    // Boolean
let value;              // Undefined
let nothing = null;     // Null
let unique = Symbol();  // Symbol
let bigNumber = 123n;   // BigInt
```

### **Non-Primitive Data Types**
1. **Object**: A collection of key-value pairs.
2. **Array**: A special kind of object used to store multiple values.
3. **Function**: Reusable blocks of code.

#### **Example**:
```javascript
let person = { name: "Alice", age: 25 };  // Object
let colors = ["red", "blue", "green"];    // Array
function greet() { return "Hello!"; }    // Function
```

---

## **Operators**

### **1. Arithmetic Operators**
Used to perform mathematical operations.
- `+` : Addition
- `-` : Subtraction
- `*` : Multiplication
- `/` : Division
- `%` : Modulus (remainder)
- `**` : Exponentiation

#### **Example**:
```javascript
let x = 5, y = 2;
console.log(x + y);  // 7
console.log(x % y);  // 1
```

### **2. Assignment Operators**
Used to assign values to variables.
- `=` : Assign
- `+=` : Add and assign
- `-=` : Subtract and assign
- `*=` : Multiply and assign
- `/=` : Divide and assign
- `%=` : Modulus and assign

#### **Example**:
```javascript
let a = 10;
a += 5;  // a = a + 5
console.log(a);  // 15
```

### **3. Comparison Operators**
Used to compare two values.
- `==` : Equal to
- `===` : Strict equal to (checks value and type)
- `!=` : Not equal to
- `!==` : Strict not equal to
- `>` : Greater than
- `<` : Less than
- `>=` : Greater than or equal to
- `<=` : Less than or equal to

#### **Example**:
```javascript
console.log(5 == "5");   // true
console.log(5 === "5");  // false
```

### **4. Logical Operators**
Used for logical operations.
- `&&` : AND
- `||` : OR
- `!` : NOT

#### **Example**:
```javascript
let x = true, y = false;
console.log(x && y);  // false
console.log(x || y);  // true
console.log(!x);      // false
```

### **5. Bitwise Operators**
Operate on the binary representation of numbers.
- `&` : AND
- `|` : OR
- `^` : XOR
- `~` : NOT
- `<<` : Left shift
- `>>` : Right shift

### **6. Ternary Operator**
Short for `if-else`.
```javascript
condition ? expression1 : expression2;
```
#### **Example**:
```javascript
let age = 18;
let status = age >= 18 ? "Adult" : "Minor";
console.log(status);  // "Adult"
```

### **7. Type Operators**
- `typeof` : Returns the type of a variable.
- `instanceof` : Checks if an object is an instance of a class.

#### **Example**:
```javascript
console.log(typeof 42);         // "number"
console.log([] instanceof Array); // true
