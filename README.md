# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  
# Date : 
# Aim:
To build a C program that prints integer, float,character, and string literals on the console using the printf() function.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside the main() function, use printf() to display each literal along with its size in bytes using sizeof() :
  
   3.1 Integer literal (e.g., 10) using `%d`
   
   3.2 Float literal (e.g., 3.14) using `%f`
   
   3.3 Character literal (e.g., 'A') using `%c`
   
   3.4 String literal (e.g., "Hello C") using `%s`
   
### Step 4: 
   Stop
# Program:
```c
#include <stdio.h>

int main() {
    // Integer literal
    int intLiteral = 10;
    printf("Integer literal: %d, Size: %lu bytes\n", intLiteral, sizeof(intLiteral));

    // Float literal
    float floatLiteral = 3.14f;
    printf("Float literal: %f, Size: %lu bytes\n", floatLiteral, sizeof(floatLiteral));

    // Character literal
    char charLiteral = 'A';
    printf("Character literal: %c, Size: %lu bytes\n", charLiteral, sizeof(charLiteral));

    // String literal
    char strLiteral[] = "Hello C";
    printf("String literal: %s, Size: %lu bytes\n", strLiteral, sizeof(strLiteral));

    return 0;
}
```
# Output:
<img width="456" height="144" alt="image" src="https://github.com/user-attachments/assets/fd6b7298-1315-4b44-ac9f-e394b5003899" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable.
# Date : 
# Aim:
  To build a C program that demonstrates the use of macro constants and constant variables.
# Algorithm:
### Step 1:
  Start  
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Define a macro constant `PI` with value `3.14159` using `#define`.
### Step 4: 
   Inside `main()`:
   
   4.1 Declare a constant integer variable `DAYS`
   
   4.2 Initialize it with the value `7`
   
### Step 5:  
  Use `printf()` to display the values of `PI` and `DAYS`.     
### Step 6:  
  Stop
# Program:
```c
#include <stdio.h>

// Macro constant
#define PI 3.14159

int main() {
    // Constant variable
    const int DAYS = 7;

    // Display values
    printf("Macro constant PI: %f\n", PI);
    printf("Constant variable DAYS: %d\n", DAYS);

    return 0;
}

```
# Output:
<img width="356" height="69" alt="image" src="https://github.com/user-attachments/assets/42ac9a8c-6238-4930-99ed-35293d74c080" />


# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
# Date : 
# Aim:
  To build a C program that declares variables of various data types—integer, float, double, and character—initializes them, and prints their values on the screen.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside main(), declare and initialize variables of types int, float, double, and char.
### Step 4: 
   Display their values using printf().
### Step 5:    
   Stop
# Program:
```c
#include <stdio.h>

int main() {
    // Declare and initialize variables of different data types
    int intVar = 25;
    float floatVar = 12.5f;
    double doubleVar = 123.456789;
    char charVar = 'C';

    // Display their values using printf()
    printf("Integer value: %d\n", intVar);
    printf("Float value: %f\n", floatVar);
    printf("Double value: %lf\n", doubleVar);
    printf("Character value: %c\n", charVar);

    return 0;
}
```
# Output:
<img width="318" height="122" alt="image" src="https://github.com/user-attachments/assets/9c461a03-aa80-4026-bd37-729f35b44be6" />

# Result:
Thus, the program was implemented and executed successfully, and the required output was obtained.

# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
# Date : 
# Aim:
  To build a C program that takes two integers as input and demonstrates the arithmetic and bitwise operations, displaying the results of each operation.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare two integer variables a and b.
### Step 4: 
   Prompt the user to enter two integers and read the input using scanf().
### Step 5:    
   Perform arithmetic operations on a and b:
   #### Sum (a + b)
   #### Difference (a - b)
   #### Product (a * b)
   #### Quotient (a / b)
   #### Remainder (a % b)
### Step 6: 
  Perform bitwise operations on a and b:
  #### AND (a &amp; b)
  #### OR (a | b)
  #### XOR (a ^ b)
  #### Left shift (a << b)
  #### Right shift (a >> b)
  #### Bitwise NOT of a (~a) and b (~b)
### Step 7:   
  Display the results of all operations using printf().
### Step 8:   
  Stop
# Program:
```c
#include <stdio.h>

int main() {
    int a, b;

    // Step 4: Input two integers
    printf("Enter two integers: ");
    scanf("%d %d", &a, &b);

    // Arithmetic operations
    printf("\n--- Arithmetic Operations ---\n");
    printf("Addition (a + b): %d\n", a + b);
    printf("Subtraction (a - b): %d\n", a - b);
    printf("Multiplication (a * b): %d\n", a * b);

    if (b != 0) { // Avoid division by zero
        printf("Division (a / b): %d\n", a / b);
        printf("Remainder (a %% b): %d\n", a % b);
    } else {
        printf("Division and Remainder not possible (b = 0)\n");
    }

    // Bitwise operations
    printf("\n--- Bitwise Operations ---\n");
    printf("AND (a & b): %d\n", a & b);
    printf("OR (a | b): %d\n", a | b);
    printf("XOR (a ^ b): %d\n", a ^ b);
    printf("Left Shift (a << 1): %d\n", a << 1);
    printf("Right Shift (a >> 1): %d\n", a >> 1);
    printf("Bitwise NOT of a (~a): %d\n", ~a);
    printf("Bitwise NOT of b (~b): %d\n", ~b);

    return 0;
}

```
# Output:
<img width="373" height="476" alt="image" src="https://github.com/user-attachments/assets/700bea58-9868-4fc7-baee-7d43232d0d17" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
# Date : 
# Aim:
  To develop and implement a C program that classifies a character as a vowel, consonant, digit, or special symbol using the ternary operator.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Input a character ch from the user.
### Step 4: 
   Check if ch is a digit ('0' to '9').
   
   If true → Print "Digit" → Go to Step 8.
   
   If false → Go to Step 5.
   
### Step 5:    
   Check if ch is an alphabet letter ('A' - 'Z' or 'a' – 'z').
   
   If true → Go to Step 6.
   
   If false → Go to Step 7.
   
### Step 6: 
   Check if ch is a vowel (a, e, i, o, u or A, E, I, O, U).
   
   If true → Print "Vowel" → Go to Step 8.
   
   If false → Print "Consonant" → Go to Step 8.
   
### Step 7:   
   Print "Special Symbol".
### Step 8:   
  Stop
# Program:
```c
#include <stdio.h>

int main() {
    char ch;

    // Step 3: Input a character
    printf("Enter a character: ");
    scanf("%c", &ch);

    // Step 4–7: Classification using ternary operator
    (ch >= '0' && ch <= '9') ? 
        printf("Digit\n") : 
        ((ch >= 'A' && ch <= 'Z') || (ch >= 'a' && ch <= 'z')) ? 
            ((ch=='A'||ch=='E'||ch=='I'||ch=='O'||ch=='U'||
              ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='u') ? 
                printf("Vowel\n") : 
                printf("Consonant\n")) 
            : 
            printf("Special Symbol\n");

    return 0;
}
```
# Output:
<img width="246" height="74" alt="image" src="https://github.com/user-attachments/assets/89e1b75b-81f8-4ab0-8476-07e0686fa8d8" />
<img width="233" height="65" alt="image" src="https://github.com/user-attachments/assets/6f5a6dfd-c511-4e0b-ae2d-978ea72d4077" />
<img width="223" height="62" alt="image" src="https://github.com/user-attachments/assets/fb418623-6f75-4ef4-ae81-417436ed844e" />
<img width="239" height="80" alt="image" src="https://github.com/user-attachments/assets/57d6eef7-5653-4ccb-8f95-f5a95be4407d" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


