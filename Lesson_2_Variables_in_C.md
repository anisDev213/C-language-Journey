
```c
#include <stdio.h>

int main() {
	 
	// variable = A reusable container for a value
	// behaves as if it were the value it contains

	int age = 25;
	int year = 2025;
	int quantity = 1;

	printf("You are %d years old\n", age);
	printf("The year is %d\n", year);
	printf("You have ordered %d x items", quantity);

	return 0;
}
```

---

## 🧩 Explanation

### 🧱 What is a Variable?
A **variable** is a **named container** that stores data in memory.  
Think of it like a labeled box in your computer’s memory — you put a value in it and can reuse or change it later.  
When you create a variable, the computer reserves a specific amount of **RAM** to hold its value.

Example:
```c
int age = 25;
```
- `int` tells the compiler what **type of data** you want to store.  
- `age` is the **variable name** (the box’s label).  
- `25` is the **value** stored inside it.

---

## 🧮 Common Data Types

| Type              | Example                       | Meaning                              | Memory size (approx.) | Format specifier |
| ----------------- | ----------------------------- | ------------------------------------ | --------------------- | ---------------- |
| `int`             | `int age = 25;`               | Whole numbers (positive or negative) | 4 bytes               | `%d`             |
| `float`           | `float price = 19.99;`        | Decimal numbers (less precise)       | 4 bytes               | `%f`             |
| `double`          | `double distance = 1234.567;` | Decimal numbers (more precise)       | 8 bytes               | `%lf`            |
| `char`            | `char grade = 'A';`           | Single character                     | 1 byte                | `%c`             |
| `_Bool` or `bool` | `bool isOn = 1;`              | Logical true (1) or false (0)        | 1 byte                | `%d`             |

*(For `bool`, include `#include <stdbool.h>`.)*

---

## 🧠 How Memory Handles Variables (Simple View)
When you declare a variable:
```c
int age = 25;
```
1. The computer **allocates 4 bytes** of memory for it (since `int` usually takes 4 bytes).
2. It assigns that memory space an **address** — a unique location (like house number).
3. The value `25` is stored inside that location.
4. When your code uses `age`, the CPU looks at that memory address to get the stored value.

So when you run:
```c
printf("You are %d years old\n", age);
```
`printf` fetches the number stored in the memory box labeled `age` and prints it.

---

## ⚙️ Output
```
You are 25 years old
The year is 2025
You have ordered 1 x items
```

---

## 💡 Notes for Memory and Variables
- Variables must have a **type** before use (C is statically typed).  
- The type determines **how much space** it uses and **how it behaves** in operations.  
- Changing a variable’s value replaces the old data in its memory location.  
- Each variable is stored at a unique address — later, you’ll learn how to access that using **pointers**.
