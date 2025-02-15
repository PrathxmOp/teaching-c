

# C Programming Course  
**By your favorite coding buddy, Prathxm**

Namaste dosto!  
Welcome to our super fun C programming journey. Yahaan hum coding ko serious tareeke se seekhenge—but masti, mazaak, aur thoda sa desi tadka bhi milega! Ready ho jao for lots of laughs and learning!

---

## Session 1: Introduction & Environment Setup

C programming ko ek dum "jhakaas" tarike se start karte hain.  
Sabse pehle, apne development environment ko set karo—GCC compiler ya koi bhi aapka favorite IDE install kar lo, warna compiler gussa ho jayega!

### Example: Hello, World!

```c
#include <stdio.h>  // Standard I/O library - yeh aapko input aur output mein help karega

int main() {        // Program ka starting point (bas, yahi se sab shuru!)
    printf("Hello, World!\n");  // Console pe yeh message chhapa do, just like saying hi to the world!
    return 0;      // Return 0 means sab sahi chal raha hai
}
```

---

## Session 2: Basic Syntax, Variables, and Data Types

Variables ko declare karna bilkul waise hi hai jaise aap apne goals set karte ho—bas, yeh code mein values store karne ke liye hota hai!

### Example: Variables & Data Types

```c
#include <stdio.h>

int main() {
    int age = 20;          // Ek integer variable
    float height = 5.9;    // Floating-point variable, jaise height ki value!
    char initial = 'J';    // Character variable, bilkul aapke naam ka pehla letter!

    printf("Age: %d\n", age);
    printf("Height: %.1f\n", height);  // Ek decimal point ke saath
    printf("Initial: %c\n", initial);
    
    return 0;
}
```

### Example: Reading Input with `scanf`

```c
#include <stdio.h>

int main() {
    int age;
    
    printf("Enter your age: ");  // Aapki umar batao!
    scanf("%d", &age);  // Input lene ke liye, bas pointer de do!
    printf("Your age is: %d\n", age);
    
    return 0;
}
```

---

## Session 3: Operators and Expressions

Operators se hum calculations karte hain—jaise paise ka hisaab, bina kisi confusion ke!

### Example: Arithmetic Operations

```c
#include <stdio.h>

int main() {
    int a = 10, b = 3;
    
    printf("a = %d, b = %d\n", a, b);
    printf("Addition: a + b = %d\n", a + b);
    printf("Subtraction: a - b = %d\n", a - b);
    printf("Multiplication: a * b = %d\n", a * b);
    printf("Division (integer division): a / b = %d\n", a / b);
    printf("Modulus: a %% b = %d\n", a % b);  // %% is used to print a literal '%'
    
    return 0;
}
```

---

## Session 4: Control Structures – Conditional Statements

Conditional statements aapko decision making mein help karte hain—jaise "agar baarish ho rahi hai to umbrella le lo, warna nikal jao!"

### Example: if-else Statement

```c
#include <stdio.h>

int main() {
    int number;
    
    printf("Enter a number: ");
    scanf("%d", &number);
    
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

### Example: switch-case Statement

```c
#include <stdio.h>

int main() {
    int day;
    
    printf("Enter a number (1-7) for a day of the week: ");
    scanf("%d", &day);
    
    switch(day) {
        case 1:
            printf("Monday\n");
            break;
        case 2:
            printf("Tuesday\n");
            break;
        // Add more cases for 3-7, because har din important hai!
        default:
            printf("Invalid day. Kya aap week mein extra din chahte ho?\n");
    }
    
    return 0;
}
```

---

## Session 5: Control Structures – Loops

Loops se ek hi kaam baar baar karna bahut aasan ho jata hai—jaise aap apne jokes ko repeat karte ho (bas, thoda dhyan se sunna!).

### Example: for Loop

```c
#include <stdio.h>

int main() {
    int i;
    
    printf("Counting from 1 to 5 using a for loop:\n");
    for (i = 1; i <= 5; i++) {
        printf("%d ", i);
    }
    printf("\n");
    
    return 0;
}
```

### Example: while Loop

```c
#include <stdio.h>

int main() {
    int i = 1;
    
    printf("Counting from 1 to 5 using a while loop:\n");
    while (i <= 5) {
        printf("%d ", i);
        i++;
    }
    printf("\n");
    
    return 0;
}
```

### Example: do-while Loop

```c
#include <stdio.h>

int main() {
    int i = 1;
    
    printf("Counting from 1 to 5 using a do-while loop:\n");
    do {
        printf("%d ", i);
        i++;
    } while (i <= 5);
    printf("\n");
    
    return 0;
}
```

---

## Session 6: Functions and Modular Programming

Functions se aap apna code chhote chhote parts mein baant sakte ho—jaise pizza slices, sabko share karne ke liye!

### Example: Factorial Function Using Recursion

```c
#include <stdio.h>

// Function prototype
int factorial(int n);

int main() {
    int number;
    
    printf("Enter a number to compute its factorial: ");
    scanf("%d", &number);
    printf("Factorial of %d is %d\n", number, factorial(number));
    
    return 0;
}

// Recursive function to compute factorial
int factorial(int n) {
    if (n == 0) {  // Base case: 0 ka factorial is 1, bilkul mummy ka pyaar!
        return 1;
    } else {
        return n * factorial(n - 1);
    }
}
```

---

## Session 7: Arrays and Strings

Arrays se aap ek variable mein multiple values store kar sakte ho—jaise doston ka group chat, sab ek saath!  
Strings basically character arrays hain jo ek null character (`\0`) pe khatam hote hain.

### Example: Arrays

```c
#include <stdio.h>

int main() {
    int numbers[5] = {10, 20, 30, 40, 50};  // Array initialization, full on value-packing!
    int i;
    
    printf("Elements of the array:\n");
    for (i = 0; i < 5; i++) {
        printf("numbers[%d] = %d\n", i, numbers[i]);
    }
    
    return 0;
}
```

### Example: Strings

```c
#include <stdio.h>

int main() {
    char greeting[] = "Hello, World!";  // String initialization
    
    printf("%s\n", greeting);  // Print the string until the null character!
    
    return 0;
}
```

---

## Session 8: Pointers

Pointers ekdam detective jaise hote hain—they store memory addresses!  
Unko samajhna thoda tricky ho sakta hai, par once you get it, it's like solving a mystery with Sherlock Holmes style!

### Example: Basic Pointers

```c
#include <stdio.h>

int main() {
    int num = 100;
    int *ptr = &num;  // Pointer ka magic: storing the address of num
    
    printf("Value of num: %d\n", num);
    printf("Address of num: %p\n", (void*)&num);
    printf("Value stored in ptr (address of num): %p\n", (void*)ptr);
    printf("Value pointed to by ptr: %d\n", *ptr);  // Dereference and get the value
    
    return 0;
}
```

---

## Session 9: Structures and Unions

Structures se aap alag alag data types ko ek group mein organize kar sakte ho—jaise ek full family, sab ek saath!  
Unions similar hota hai, par sab members same memory space share karte hain—jaise family budget, sab ek hi pot se khate hain!

### Example: Structure

```c
#include <stdio.h>

struct Student {
    int id;
    char name[50];
    float gpa;
};

int main() {
    struct Student student1 = {101, "Alice", 3.8};
    
    printf("Student ID: %d\n", student1.id);
    printf("Student Name: %s\n", student1.name);
    printf("Student GPA: %.2f\n", student1.gpa);
    
    return 0;
}
```

### Example: Union

```c
#include <stdio.h>

union Data {
    int i;
    float f;
    char str[20];
};

int main() {
    union Data data;
    
    data.i = 10;
    printf("data.i: %d\n", data.i);
    
    // Changing one member affects others, kyunki sab ek hi memory space share karte hain!
    data.f = 220.5;
    printf("data.f: %.2f\n", data.f);
    
    return 0;
}
```

---

## Session 10: Dynamic Memory Allocation

Dynamic memory allocation se aap runtime pe extra memory mangwa sakte ho—bilkul pizza order karne jaise, extra cheese hamesha maangna chahiye!

### Example: Allocating & Freeing Memory

```c
#include <stdio.h>
#include <stdlib.h>  // For malloc and free

int main() {
    int n, i;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    
    // Dynamically allocate memory for n integers
    int *arr = (int*)malloc(n * sizeof(int));
    if (arr == NULL) {
        printf("Memory allocation failed. Arre, memory khatam!\n");
        return 1;
    }
    
    // Initialize and display the array
    for (i = 0; i < n; i++) {
        arr[i] = i * 10;
    }
    
    printf("Array elements:\n");
    for (i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }
    printf("\n");
    
    // Free the allocated memory
    free(arr);
    
    return 0;
}
```

---

## Session 11: File I/O

File I/O se aap files ke saath interact kar sakte ho—jaise computer ki diary padhna aur likhna, but bina gossip ke!

### Example: Writing & Reading from a File

```c
#include <stdio.h>

int main() {
    FILE *fp;
    char data[100];

    // Writing to a file
    fp = fopen("example.txt", "w");  // Open file in write mode
    if (fp == NULL) {
        printf("Error opening file for writing.\n");
        return 1;
    }
    fprintf(fp, "Hello, file I/O! Yeh Prathxm ka message hai.\n");  // Write to the file
    fclose(fp);
    
    // Reading from the file
    fp = fopen("example.txt", "r");  // Open file in read mode
    if (fp == NULL) {
        printf("Error opening file for reading.\n");
        return 1;
    }
    while (fgets(data, 100, fp) != NULL) {
        printf("%s", data);
    }
    fclose(fp);
    
    return 0;
}
```

---

## Session 12: Preprocessor Directives and Macros

Preprocessor directives code compile hone se pehle run hote hain—bilkul morning coffee jaise, bina iske din shuru nahi hota!

### Example: Using a Macro

```c
#include <stdio.h>
#define PI 3.14159  // Define a constant for PI

int main() {
    float radius = 5.0;
    float area = PI * radius * radius;
    
    printf("Area of a circle with radius %.1f is %.2f\n", radius, area);
    return 0;
}
```

---

## Session 13: Debugging and Error Handling

Debugging matlab code ki galtiyon ko pakadna—jaise mummy pakad leti hain jab aap chhup ke kuch karte ho!  
Is session mein aap error messages ko samjhenge aur unhe fix karne ka tareeka seekhenge.

### Example: Identifying an Error

```c
#include <stdio.h>

int main() {
    int num = 10;
    // Yahan semicolon missing hai—compilation error ho jayega!
    printf("Number is %d\n", num)
    return 0;
}
```

*Tip:* Dhyan se code padho, choti choti galtiyan bhi badi problem bana deti hain. Use debugging tools like gdb to help out!

---

## Session 14: Final Project and Review

Ab sab sessions ka ultimate test time aa gaya hai!  
Apna final project taiyaar karo—chahe woh ek simple calculator ho, ek chota game ho, ya koi data processing application. Project complete karke, batao kaunse topics use kiye aur kya challenges aaye.  

*Final Tips:*  
- Code examples ke saath experiment karo.  
- Naye values try karo aur alag alag scenarios explore karo.  
- Agar koi doubt ho, toh pucho—main (Prathxm) hamesha yahan hoon help ke liye!

---

Happy coding, keep smiling, and may your bugs be few!  
**— Prathxm**
