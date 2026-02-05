## **Part 1 – Logical & Ternary Operator**
### **Q1: Check number between 10 and 50**

```js
let num = 25;

if (num >= 10 && num <= 50) {
  console.log("Valid Number");
} else {
  console.log("Invalid Number");
}
```

---

### **Q2: Login eligibility using logical AND**

```js
let username = "admin";
let password = "1234";

if (username === "admin" && password === "1234") {
  console.log("Login Successful");
} else {
  console.log("Invalid Login");
}
```

---

### **Q3: Even or Odd using ternary operator**

```js
let number = 7;
let result = (number % 2 === 0) ? "Even" : "Odd";
console.log(result);
```

---

### **Q4: Output & explanation**

```js
console.log((10 === "10") || (5 > 2) && !(3 < 1));
```

**Step-by-step:**

1. `10 === "10"` → `false` (strict comparison)
2. `5 > 2` → `true`
3. `3 < 1` → `false`
4. `!(false)` → `true`
5. `true && true` → `true`
6. `false || true` → `true`

 **Final Output:** `true`

---

## **Part 2 – Type Conversion**

### **Q5: Output & explanation**

```js
console.log("5" + 2); // "52" → string concatenation
console.log("5" - 2); // 3 → string converted to number
console.log("5" * 2); // 10 → numeric operation
console.log("5" / 2); // 2.5 → numeric operation
```

---

### **Q6: Explicit Conversion**

```js
let value = "100";

let numValue = Number(value);
let boolValue = Boolean(value);

console.log(numValue);  // 100
console.log(boolValue); // true
```

---

### **Q7: Boolean conversion output**

```js
console.log(Boolean(""));   // false
console.log(Boolean(" "));  // true
console.log(Boolean(0));    // false
console.log(Boolean([]));   // true
```

**Why?**

* `""` → empty string → false
* `" "` → non-empty string → true
* `0` → false
* `[]` → object → true

---

## **Part 3 – Conditional Statements**

### **Q8: Grade program**

```js
let marks = 78;

if (marks >= 90) {
  console.log("Grade A");
} else if (marks >= 75) {
  console.log("Grade B");
} else if (marks >= 50) {
  console.log("Grade C");
} else {
  console.log("Fail");
}
```

---

### **Q9: Traffic signal using switch**

```js
let signal = "green";

switch (signal) {
  case "red":
    console.log("Stop");
    break;
  case "yellow":
    console.log("Ready");
    break;
  case "green":
    console.log("Go");
    break;
  default:
    console.log("Invalid Signal");
}
```

---

### **Q10: Nested If – Eligibility Check**

```js
let age = 20;
let height = 165;
let weight = 55;

if (age >= 18) {
  if (height >= 160) {
    if (weight >= 50) {
      console.log("Selected");
    } else {
      console.log("Weight condition failed");
    }
  } else {
    console.log("Height condition failed");
  }
} else {
  console.log("Age condition failed");
}
```

---

## **Part 4 – Loops**

### **Q11: Print 1 to 20**

```js
for (let i = 1; i <= 20; i++) {
  console.log(i);
}
```

---

### **Q12: Print odd numbers (1–20)**

```js
for (let i = 1; i <= 20; i++) {
  if (i % 2 !== 0) {
    console.log(i);
  }
}
```

---

### **Q13: While loop (10 to 1)**

```js
let i = 10;
while (i >= 1) {
  console.log(i);
  i--;
}
```

---

### **Q14: Do-while loop (1 to 5)**

```js
let i = 1;
do {
  console.log(i);
  i++;
} while (i <= 5);
```

---

### **Q15: for-of loop**

```js
let word = "STACKLY";

for (let char of word) {
  console.log(char);
}
```

---

### **Q16: for-in loop**

```js
let student = {
  name: "Arun",
  course: "MERN",
  duration: "6 months"
};

for (let key in student) {
  console.log(key + " : " + student[key]);
}
```

---

## **Real-Time Questions**

### **RT-1: Login System (Logical + Ternary)**

```js
let username = "admin";
let password = "1234";

let result = (username === "admin" && password === "1234")
  ? "Login Success"
  : "Invalid Credentials";

console.log(result);
```

---

### **RT-2: Salary Bonus System**

```js
let salary = 60000;
let experience = 4;

if (salary > 50000 && experience > 3) {
  console.log("Eligible for bonus");
} else {
  console.log("Not eligible");
}
```

---

### **RT-3: Shopping Discount**

```js
let amount = 3000;

if (amount >= 5000) {
  console.log("20% Discount");
} else if (amount >= 2000) {
  console.log("10% Discount");
} else {
  console.log("No Discount");
}
```

---

### **RT-4: Even/Odd Counter (1–50)**

```js
let count = 0;

for (let i = 1; i <= 50; i++) {
  if (i % 2 === 0) {
    count++;
  }
}

console.log("Even numbers count:", count);
```

---

### **RT-5: Dynamic Greeting System**

```js
let hour = 18;

if (hour >= 1 && hour <= 6) {
  console.log("Good Morning");
} else if (hour <= 12) {
  console.log("Morning");
} else if (hour <= 16) {
  console.log("Good Afternoon");
} else if (hour <= 19) {
  console.log("Good Evening");
} else {
  console.log("Good Night");
}
