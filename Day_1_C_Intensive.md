<img src="https://r2cdn.perplexity.ai/pplx-full-logo-primary-dark%402x.png" class="logo" width="120"/>

# So, today onwards, I'm going to start. I'll regularly come here and ask you, according to the day. Kindly give me all the best tips and concepts with programmes for my learning

Fantastic! 💻 Let's begin **Day 1** with foundational concepts. Reply with "Day 1" or "Proceed to Day 1" when ready, and I'll provide a structured lesson with code examples, common interview questions, and practice tasks.

---

### **Day 1: Introduction \& Setup**

**Goal**: Understand C syntax, write your first program, and set up your coding environment.

#### **Key Concepts**

1. **Structure of a C Program**:

```c
#include <stdio.h>  // Preprocessor directive for I/O functions
int main() {        // Entry point of the program
    printf("Hello, World!\n");  
    return 0;       // Exit status
}
```

    - `#include` includes header files (e.g., `stdio.h` for input/output).
    - `main()` is the starting function executed by the OS.
2. **Compilation Process**:
    - Use `gcc hello.c -o hello` (Linux/Mac) or a compiler like Code::Blocks/DevC++ (Windows).
    - Run with `./hello` (Terminal) or double-click the executable.
3. **Basic Syntax Rules**:
    - Case-sensitive (e.g., `Main` ≠ `main`).
    - Statements end with `;`.
    - Use `//` for single-line comments or `/* ... */` for multi-line.

---

#### **Common Pitfalls (Interview Focus)**

- Missing semicolons or braces.
- Forgetting `\n` in `printf` for newlines.
- Using `void main()` instead of `int main()` (not standard in modern C).

---

#### **Practice Programs**

1. **Hello, World!**:
Modify the program to print:

```
Hello, [Your Name]!
Today is Day 1 of my C journey.
```

2. **Basic Arithmetic**:

```c
#include <stdio.h>
int main() {
    int a = 5, b = 3;
    printf("Sum: %d\n", a + b);
    printf("Product: %d\n", a * b);
    return 0;
}
```


---

#### **Interview-Style Question**

**Q**: Why is `main()` declared as `int main()` and not `void main()`?
**A**: The C standard requires `main()` to return an `int` exit status to the OS (0 = success, non-zero = error). `void main()` is non-standard and compiler-dependent.

---

#### **Action Items for Today**

✅ Write and run 3 variations of "Hello, World!" with different text.
✅ Experiment with arithmetic operations (subtract, divide, modulus).
✅ Research: What happens if you omit `return 0;` in `main()`?

Reply with **Day 1 Done** when finished, and I’ll provide Day 2! 🚀

---
PS: Stay consistent – even 2 hours of focused practice daily will build momentum! 💪

