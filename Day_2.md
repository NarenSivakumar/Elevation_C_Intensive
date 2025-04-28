Proceed with Day 2

Absolutely! Let’s dive into **Day 2: Variables, Data Types, and Operators**-crucial topics for both C fundamentals and interview success.

---

## **Day 2: Variables, Data Types, and Operators**

### **1. Variables in C**
- **Definition:** Named storage for data that can be modified during program execution.
- **Declaration & Initialization:**
  ```c
  int age;         // Declaration
  age = 25;        // Initialization
  float salary = 35000.50; // Declaration + Initialization
  ```

### **2. Data Types**
- **Primary Data Types:**
  | Type    | Size (Typical) | Example        |
  |---------|----------------|----------------|
  | int     | 2 or 4 bytes   | int x = 10;    |
  | float   | 4 bytes        | float y = 2.5; |
  | double  | 8 bytes        | double z = 3.14;|
  | char    | 1 byte         | char c = 'A';  |

- **Modifiers:** `short`, `long`, `signed`, `unsigned`
  ```c
  unsigned int u = 100;
  long int l = 1234567890;
  ```

### **3. Constants**
- **Using `#define`:**  
  ```c
  #define PI 3.14159
  ```
- **Using `const`:**
  ```c
  const int DAYS = 7;
  ```

### **4. Operators**
- **Arithmetic:** `+`, `-`, `*`, `/`, `%`
- **Relational:** `==`, `!=`, `>`, `<`, `>=`, `<=`
- **Logical:** `&&`, `||`, `!`
- **Assignment:** `=`, `+=`, `-=`, `*=`, `/=`
- **Bitwise:** `&`, `|`, `^`, `~`, `<<`, `>>`
- **Increment/Decrement:** `++`, `--`

#### **Example:**
```c
int a = 5, b = 2;
printf("%d\n", a + b); // 7
printf("%d\n", a % b); // 1
printf("%d\n", a > b); // 1 (true)
printf("%d\n", a == b); // 0 (false)
```

---

## **Interview Tips & Common Pitfalls**
- **Uninitialized variables** can cause unpredictable results.
- **Integer division:** `5 / 2` gives `2`, not `2.5`.
- **Type conversion:** Assigning `float` to `int` truncates the decimal.
- **Bitwise vs. Logical:** `&` is bitwise AND, `&&` is logical AND.

---

## **Practice Programs**

### **1. Simple Calculator**
```c
#include <stdio.h>
int main() {
    int a = 12, b = 5;
    printf("Sum: %d\n", a + b);
    printf("Difference: %d\n", a - b);
    printf("Product: %d\n", a * b);
    printf("Quotient: %d\n", a / b);
    printf("Remainder: %d\n", a % b);
    return 0;
}
```

### **2. Swap Two Numbers (Using a Temporary Variable)**
```c
#include <stdio.h>
int main() {
    int x = 10, y = 20, temp;
    temp = x;
    x = y;
    y = temp;
    printf("x = %d, y = %d\n", x, y);
    return 0;
}
```

### **3. Bitwise Operator Example**
```c
#include <stdio.h>
int main() {
    int a = 5, b = 3;
    printf("a & b = %d\n", a & b); // 1
    printf("a | b = %d\n", a | b); // 7
    printf("a ^ b = %d\n", a ^ b); // 6
    return 0;
}
```

---

## **Interview-Style Questions**

1. **What is the difference between `float` and `double` in C?**
   - `float` is 4 bytes (single precision), `double` is 8 bytes (double precision), so `double` can store larger and more precise values.

2. **What happens if you assign a `float` to an `int` variable?**
   - The decimal part is truncated, not rounded.

3. **What is the output?**
   ```c
   int a = 5, b = 2;
   float c = a / b;
   printf("%f", c);
   ```
   **Answer:** Output is `2.000000` because `a / b` is integer division. To get `2.5`, use `float c = (float)a / b;`

4. **What is the difference between `=` and `==`?**
   - `=` assigns a value, `==` compares values.

5. **What is the output?**
   ```c
   int a = 10;
   printf("%d", a++ + ++a);
   ```
   **Answer:** Output is `22`. (a++ is 10, then a becomes 11, ++a makes it 12, so 10 + 12).

---

## **Tasks for Today**
- ✅ Write and run the sample programs above.
- ✅ Try declaring variables with different data types and print their values.
- ✅ Experiment with all operators (`+`, `-`, `*`, `/`, `%`, `&`, `|`, etc.).
- ✅ Write a program to swap two numbers without using a temporary variable (hint: use `+` and `-` or XOR).

---

Let me know when you’re done with Day 2, or if you want more interview questions or coding challenges for today’s topics! 🚀

