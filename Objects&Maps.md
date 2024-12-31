# JavaScript Notes: Objects & Maps, Destructuring

## **Objects**
Objects are collections of key-value pairs.

### **1. Creating Objects**
#### Syntax:
```javascript
const objectName = {
    key1: value1,
    key2: value2,
};
```
#### Example:
```javascript
const person = {
    name: "Alice",
    age: 25,
    greet: function() {
        return `Hello, ${this.name}`;
    },
};
console.log(person.greet());
```

### **2. Accessing Properties**
- **Dot Notation**: `objectName.key`
- **Bracket Notation**: `objectName["key"]`

#### Example:
```javascript
console.log(person.name);      // "Alice"
console.log(person["age"]);   // 25
```

### **3. Adding and Modifying Properties**
#### Example:
```javascript
person.city = "New York";   // Adding
person.age = 30;            // Modifying
console.log(person);
```

### **4. Deleting Properties**
#### Example:
```javascript
delete person.city;
console.log(person);
```

### **5. Methods**
Functions stored in an object.

#### Example:
```javascript
const calculator = {
    add: function(a, b) {
        return a + b;
    },
};
console.log(calculator.add(2, 3));  // 5
```

---

## **Maps**
`Map` is a collection of key-value pairs where keys can be any data type.

### **1. Creating a Map**
#### Syntax:
```javascript
const map = new Map();
```
#### Example:
```javascript
const map = new Map([
    ["name", "Alice"],
    ["age", 25],
]);
```

### **2. Map Methods**
- **`set(key, value)`**: Adds or updates a key-value pair.
- **`get(key)`**: Retrieves the value for a key.
- **`has(key)`**: Checks if a key exists.
- **`delete(key)`**: Removes a key-value pair.
- **`clear()`**: Removes all key-value pairs.
- **`size`**: Returns the number of entries.

#### Example:
```javascript
map.set("city", "New York");
console.log(map.get("name"));   // "Alice"
console.log(map.has("age"));   // true
map.delete("age");
console.log(map.size);          // 2
```

### **3. Iterating Over a Map**
#### Example:
```javascript
for (const [key, value] of map) {
    console.log(`${key}: ${value}`);
}
```

---

## **Destructuring**
Destructuring allows unpacking values from arrays or properties from objects into distinct variables.

### **1. Array Destructuring**
#### Syntax:
```javascript
const [var1, var2] = array;
```
#### Example:
```javascript
const colors = ["red", "green", "blue"];
const [first, second] = colors;
console.log(first);   // "red"
console.log(second);  // "green"
```

### **2. Default Values in Array Destructuring**
#### Example:
```javascript
const [a = 1, b = 2] = [];
console.log(a);   // 1
console.log(b);   // 2
```

### **3. Object Destructuring**
#### Syntax:
```javascript
const { key1, key2 } = object;
```
#### Example:
```javascript
const person = {
    name: "Alice",
    age: 25,
};
const { name, age } = person;
console.log(name);  // "Alice"
console.log(age);   // 25
```

### **4. Renaming Variables**
#### Example:
```javascript
const { name: fullName } = person;
console.log(fullName);  // "Alice"
```

### **5. Nested Destructuring**
#### Example:
```javascript
const person = {
    name: "Alice",
    address: {
        city: "New York",
        zip: 10001,
    },
};
const {
    address: { city, zip },
} = person;
console.log(city);  // "New York"
console.log(zip);   // 10001
```

### **6. Destructuring with Default Values**
#### Example:
```javascript
const { name, country = "USA" } = person;
console.log(country);  // "USA"
```

### **7. Combining Rest with Destructuring**
#### Example:
```javascript
const { name, ...rest } = person;
console.log(rest);  // { address: { city: "New York", zip: 10001 } }
