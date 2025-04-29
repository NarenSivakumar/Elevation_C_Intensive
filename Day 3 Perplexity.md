<img src="https://r2cdn.perplexity.ai/pplx-full-logo-primary-dark%402x.png" class="logo" width="120"/>

# with detailes

Absolutely! Here’s a detailed **Day 3 C Programming Lesson** with explanations, code, and comments for each topic and exercise.

---

## Day 3: Control Statements and Loops in C (With Detailed Explanations)


---

### 1. **If-Else Statements**

#### **What is it?**

The `if-else` statement allows your program to make decisions based on conditions.

#### **Example: Check if a Number is Positive, Negative, or Zero**

```c
#include <stdio.h>

int main() {
    int number;
    printf("Enter a number: ");
    scanf("%d", &number); // Reads user input

    if (number > 0) {
        printf("The number is positive.\n");
    } else if (number < 0) {
        printf("The number is negative.\n");
    } else {
        printf("The number is zero.\n");
    }
    return 0;
}
```

**Explanation:**

- The program reads an integer from the user.
- It checks if the number is greater than, less than, or equal to zero and prints the result.

---

### 2. **Switch Statement**

#### **What is it?**

The `switch` statement lets you choose between multiple options based on the value of a variable.

#### **Example: Simple Menu**

```c
#include <stdio.h>

int main() {
    int choice;
    printf("Enter a number between 1 and 3: ");
    scanf("%d", &choice);

    switch (choice) {
        case 1:
            printf("You chose one.\n");
            break;
        case 2:
            printf("You chose two.\n");
            break;
        case 3:
            printf("You chose three.\n");
            break;
        default:
            printf("Invalid choice.\n");
    }
    return 0;
}
```

**Explanation:**

- The program asks for a number.
- Depending on the input, it prints a different message.

---

### 3. **For Loop**

#### **What is it?**

A `for` loop repeats a block of code a specific number of times.

#### **Example: Print Numbers 1 to 5**

```c
#include <stdio.h>

int main() {
    int i;
    for (i = 1; i <= 5; i++) {
        printf("Iteration %d\n", i);
    }
    return 0;
}
```

**Explanation:**

- The loop starts at 1 and ends at 5.
- Each iteration prints the current value of `i`.

---

### 4. **While Loop**

#### **What is it?**

A `while` loop repeats a block of code as long as a condition is true.

#### **Example: Print Numbers 1 to 5**

```c
#include <stdio.h>

int main() {
    int count = 1;
    while (count <= 5) {
        printf("Count is %d\n", count);
        count++;
    }
    return 0;
}
```

**Explanation:**

- The loop continues as long as `count` is less than or equal to 5.
- `count` is incremented each time.

---

### 5. **Do-While Loop**

#### **What is it?**

A `do-while` loop is similar to a `while` loop, but it runs the code block at least once.

#### **Example: Print Numbers 1 to 5**

```c
#include <stdio.h>

int main() {
    int num = 1;
    do {
        printf("Number: %d\n", num);
        num++;
    } while (num <= 5);
    return 0;
}
```

**Explanation:**

- The loop prints the number and then checks the condition.
- It always runs at least once, even if the condition is false initially.

---

## Day 3 Exercises (With Solutions)

### **Exercise 1: Even or Odd Using If-Else**

```c
#include <stdio.h>

int main() {
    int num;
    printf("Enter an integer: ");
    scanf("%d", &num);

    if (num % 2 == 0) {
        printf("%d is even.\n", num);
    } else {
        printf("%d is odd.\n", num);
    }
    return 0;
}
```

**Explanation:**

- `%` is the modulo operator; `num % 2` checks if the number is divisible by 2.

---

### **Exercise 2: Multiplication Table Using For Loop**

```c
#include <stdio.h>

int main() {
    int num, i;
    printf("Enter a number to print its multiplication table: ");
    scanf("%d", &num);

    printf("Multiplication table of %d:\n", num);
    for (i = 1; i <= 10; i++) {
        printf("%d x %d = %d\n", num, i, num * i);
    }
    return 0;
}
```

**Explanation:**

- The loop runs from 1 to 10, printing each line of the multiplication table.

---

### **Exercise 3: Calculator Using Switch-Case**

```c
#include <stdio.h>

int main() {
    int choice;
    float a, b, result;

    printf("Menu:\n");
    printf("1. Add\n");
    printf("2. Subtract\n");
    printf("3. Multiply\n");
    printf("4. Divide\n");
    printf("Enter your choice (1-4): ");
    scanf("%d", &choice);

    printf("Enter two numbers: ");
    scanf("%f %f", &a, &b);

    switch (choice) {
        case 1:
            result = a + b;
            printf("Result: %.2f\n", result);
            break;
        case 2:
            result = a - b;
            printf("Result: %.2f\n", result);
            break;
        case 3:
            result = a * b;
            printf("Result: %.2f\n", result);
            break;
        case 4:
            if (b != 0) {
                result = a / b;
                printf("Result: %.2f\n", result);
            } else {
                printf("Error: Division by zero!\n");
            }
            break;
        default:
            printf("Invalid choice!\n");
    }
    return 0;
}
```

**Explanation:**

- The program displays a menu and asks for a choice.
- It then asks for two numbers and performs the selected operation.
- Division checks for division by zero to avoid errors.

---

## **Summary**

- **If-else**: For conditional branching.
- **Switch-case**: For multiple choices.
- **Loops**: For repeating tasks (`for`, `while`, `do-while`).
- **Practice**: Try modifying the examples or creating your own!

If you need more exercises or have questions on any topic, just ask!

