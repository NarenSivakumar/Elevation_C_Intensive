** What if I omit return 0; in main functions?
The Answer is: based on the compiler the output differs. If the compiler is old version means, it'll show undefined behaviour. 
if the compiler newer one means, compiler will take implicitly, and compiles the program properly.

* Why is main function declared as int not void?
  Ans: 👉 Because main() is the starting point of the program, and after the program finishes, it must return a status code to the operating system.
      -> int main() means main will return an integer value.
      -> That returned value tells the OS whether the program ran successfully or failed.
    Conclusion: If main() were void, it would not return any status — the OS would have no idea whether the program succeeded or failed.

* What is token in C program?
  Ans: Token is the smallest individual unit in C program.
  like; identifiers, keywords, constants, operators, spl char, strings.

  --> Link : https://www.perplexity.ai/search/schedule-me-a-c-program-intens-LH1LtHzOTXiKP9RNMzkxIw#2 
