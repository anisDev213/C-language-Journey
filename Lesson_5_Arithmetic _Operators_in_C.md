
## 🏷️ Arithmetic Operators in C

Arithmetic operators are used to perform basic mathematical operations:

- `+` Addition
- `-` Subtraction
- `*` Multiplication
- `/` Division (integer division if both operands are integers)
- `%` Modulus (remainder after integer division)
- `++` Increment by 1
- `--` Decrement by 1[^1][^3][^10]

***
## ⚡ Compound Assignment Operators

These combine an operation with assignment, simplifying code.


| Compound Operator | Expanded Form | Example |
| :-- | :-- | :-- |
| `x += y;` | `x = x + y;` | Increases x by y |
| `x -= y;` | `x = x - y;` | Decreases x by y |
| `x *= y;` | `x = x * y;` | Multiplies x by y |
| `x /= y;` | `x = x / y;` | Divides x by y |
| `x %= y;` | `x = x % y;` | Remainder assignment |

Example from the code:

- `x += 2;` is the same as `x = x + 2;`
- `x -= 2;` is the same as `x = x - 2;`
- `x *= 2;` is the same as `x = x * 2;`
- `x /= 2;` is the same as `x = x / 2;`
- After these steps, `z = x;` assigns the resulting value of x to z.

***
## 📝 Example Calculation Step-by-Step

With initial values:

- `x = 10`

Operations:

- `x += 2;` → `x = 12`
- `x -= 2;` → `x = 10`
- `x *= 2;` → `x = 20`
- `x /= 2;` → `x = 10`
- `z = x;`   → `z = 10`

Final output: `10`

***
## 💡 Key Points

- Use arithmetic operators for calculations.
- Use compound assignment for cleaner, shorter code.
- `printf("%d", z);` prints the final value of z.
- When working with integers, division truncates any decimal part (e.g., `7 / 2` gives `3`).[^3][^10]

***
## 🔗 Additional Reading
[^2]: https://www.programiz.com/c-programming/c-operators




