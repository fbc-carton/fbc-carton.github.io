Here's a **detailed tutorial for JavaScript** to help beginners learn from the basics. Each section builds upon the last, so it's best to follow sequentially.

---

## **1. Introduction to JavaScript**

JavaScript is a versatile, high-level programming language that runs in web browsers and can be used to create interactive web pages, backend servers, and more.

### **How to Use JavaScript**
1. **Inline Script in HTML**:
   ```html
   <script>
       alert('Hello, World!');
   </script>
   ```
2. **External File**:
   Save JavaScript in a `.js` file and link it in an HTML file:
   ```html
   <script src="script.js"></script>
   ```

---

## **2. Basic Syntax**

### **Variables**
Variables store data. Use `let`, `const`, or `var` (avoid `var` in modern JavaScript).
```javascript
let name = "John"; // Can be reassigned
const age = 25;    // Cannot be reassigned
```

### **Data Types**
1. **String**: Text inside quotes.
   ```javascript
   let message = "Hello!";
   ```
2. **Number**: Integers and decimals.
   ```javascript
   let price = 19.99;
   ```
3. **Boolean**: `true` or `false`.
   ```javascript
   let isAvailable = true;
   ```
4. **Null**: Explicitly empty value.
   ```javascript
   let data = null;
   ```
5. **Undefined**: Not yet assigned a value.
   ```javascript
   let result;
   ```

---

### **Comments**
```javascript
// Single-line comment
/*
   Multi-line comment
*/
```

---

## **3. Operators**

### **Arithmetic Operators**
```javascript
let sum = 5 + 3;    // 8
let diff = 5 - 3;   // 2
let product = 5 * 3; // 15
let quotient = 5 / 3; // 1.67
let remainder = 5 % 3; // 2
```

### **Comparison Operators**
```javascript
console.log(5 > 3);  // true
console.log(5 == "5"); // true (value equality)
console.log(5 === "5"); // false (strict equality)
```

---

## **4. Control Structures**

### **Conditional Statements**
```javascript
let age = 18;

if (age >= 18) {
    console.log("You can vote.");
} else {
    console.log("You cannot vote.");
}
```

### **Switch Statement**
```javascript
let fruit = "apple";

switch (fruit) {
    case "apple":
        console.log("Apples are $2.");
        break;
    case "banana":
        console.log("Bananas are $1.");
        break;
    default:
        console.log("Unknown fruit.");
}
```

---

## **5. Loops**

### **For Loop**
```javascript
for (let i = 0; i < 5; i++) {
    console.log(i);
}
```

### **While Loop**
```javascript
let count = 0;

while (count < 5) {
    console.log(count);
    count++;
}
```

### **For-Of Loop (for arrays)**
```javascript
let colors = ["red", "blue", "green"];

for (let color of colors) {
    console.log(color);
}
```

---

## **6. Functions**

### **Function Declaration**
```javascript
function greet(name) {
    return `Hello, ${name}!`;
}

console.log(greet("Alice")); // Hello, Alice!
```

### **Arrow Functions**
```javascript
const add = (a, b) => a + b;

console.log(add(2, 3)); // 5
```

---

## **7. Arrays and Objects**

### **Arrays**
```javascript
let fruits = ["apple", "banana", "cherry"];

fruits.push("date"); // Add to the end
console.log(fruits[1]); // Access by index
```

### **Objects**
```javascript
let person = {
    name: "John",
    age: 30,
    greet() {
        console.log(`Hi, I am ${this.name}`);
    }
};

console.log(person.name); // Access property
person.greet(); // Call method
```

---

## **8. DOM Manipulation**
The DOM allows JavaScript to interact with HTML.

### **Select Elements**
```javascript
let element = document.getElementById("myElement");
let buttons = document.querySelectorAll(".button");
```

### **Modify Elements**
```javascript
element.textContent = "New text";
element.style.color = "blue";
```

### **Add Events**
```javascript
let button = document.querySelector("button");

button.addEventListener("click", () => {
    alert("Button clicked!");
});
```

---

## **9. Debugging**
Use the browser's **Developer Tools** (usually F12) to debug your scripts. Add breakpoints or log output with:
```javascript
console.log("Debugging");
```

---

## **10. Example Project: Counter**
### HTML:
```html
<button id="decrement">-</button>
<span id="count">0</span>
<button id="increment">+</button>
```

### JavaScript:
```javascript
let count = 0;

document.getElementById("increment").addEventListener("click", () => {
    count++;
    document.getElementById("count").textContent = count;
});

document.getElementById("decrement").addEventListener("click", () => {
    count--;
    document.getElementById("count").textContent = count;
});
```

---

This tutorial covers the **fundamentals of JavaScript**. Practice these concepts to solidify your understanding, and feel free to ask for advanced topics when you're ready!