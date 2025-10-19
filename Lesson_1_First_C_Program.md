

```c
#include <stdio.h>

int main() {
	 
	// this is my first comment

	/*
	this is multlines comment
	see ?
	*/

	printf("Hello World\n");
	printf("this is my first c programm");

	return 0;
}
```

---

## 🧩 Explanation

### 1. `#include <stdio.h>`
This line **includes the Standard Input Output library**.  
It gives access to functions like `printf()` and `scanf()` that let you display and take input.  
Without including it, the compiler wouldn’t recognize `printf()`.

---

### 2. `int main() { ... }`
Every C program **starts executing from the `main()` function**.  
`int` means the function returns an integer value to the operating system.  
The **curly braces `{ }`** define the start and end of the function’s body — where your program’s logic lives.

---

### 3. Comments
Comments are **ignored by the compiler**, they’re just notes for humans.  

- `//` for **single-line** comments.  
- `/* ... */` for **multi-line** comments.  

They help explain your code — useful when you revisit it later or when others read it.

---

### 4. `printf("Hello World\n");`
`printf()` prints text to the screen.  
The text inside quotes `"..."` is called a **string literal**.  
`\n` adds a **new line**, so the next printed text appears on a new line.

---

### 5. `return 0;`
This ends the `main()` function and sends a **status code** back to the system.  
Returning `0` usually means **the program ran successfully**.

---

## 🧭 Output

```
Hello World
this is my first c programm
```

*(Note: “programm” has an extra ‘m’ — in English it’s “program,” but the compiler doesn’t care.)*

---

## 💡 Key Ideas to Remember
- Every C program starts with `main()`.  
- Use semicolons `;` to end each statement.  
- Comments don’t affect execution — they’re for humans.  
- `#include <stdio.h>` is essential for input/output functions.
