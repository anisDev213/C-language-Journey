***
## 🏷️ What Are Format Specifiers?

- **Format specifiers** are special tokens used in `printf` (and similar functions) in C.
- They always start with a `%` followed by a character indicating the data type, plus optional *modifiers*.
- **Purpose:** Control how data is displayed or interpreted.

***
## 🛠️ Commonly Used Modifiers

### 1. **Width**

- Sets the minimum number of characters for output.
- Example: `%4d` → print integer in 4 spaces.


### 2. **Zero Padding**

- Use `0` before width for leading zeroes.
- Example: `%04d` → for `num1 = 1` prints `0001`.
- Good for aligning numbers or IDs.


### 3. **Left Alignment**

- Use `-` to left-align content.
- Example: `%-4d` → for `num2 = 10` prints `10` with spaces to the right.
- Useful for tabular layouts.


### 4. **Sign**

- Use `+` to always show sign, even if positive.
- Example: `%+4d` → for `num3 = -100` prints `-100`. For positives, will show `+`.


### 5. **Precision (for floats)**

- `%.nf` sets decimal precision to `n` digits.
- Example: `%.2f` prints 2 decimal places.


### 6. **Combined width, sign, and precision (floats)**

- Example: `%+7.2f` →
    - `+` shows sign
    - `7` width
    - `.2` for two decimal places
    - For `price1 = 123.99` prints `+123.99` right-aligned in 7 spaces.
- `%+7.1f` → same as above, but only one decimal digit (`+124.0` when rounded).

***
## 📝 Example Outputs

```c
printf("%04d\n", 1);      // 0001
printf("%-4d\n", 10);     // 10  
printf("%+4d\n", -100);   // -100
printf("%+7.2f\n", 123.99); // +123.99
printf("%+7.1f\n", 123.99); // +124.0
```


***
## 💡 Study Prompts

- Try changing the width or precision. How does the output change?
- How do different flags (`+`, `-`, `0`) combine?
- What happens if the number is too big for the width?

***
## 🗝️ Key Takeaways

- Format specifiers = flexibly control printed output.
- Combine modifiers for customized formatting.
- Critical for making nicely formatted console tables, reports, logs, etc.

