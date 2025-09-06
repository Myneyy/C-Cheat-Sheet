# C++ Cheat Sheet

---

## Introduction
This repository provides a C++ Cheat Sheet designed for beginners.
It was originally created as a personal learning resource, but it can also serve as a quick reference for others who are starting with C++.

---

## Drop a Star
Feel free to use and share this Cheat Sheet.If it helped you, please leave a ⭐.

---

## How to Use
Click on the link for your specific topic and you will be taken directly there, or simply scroll through.

---

## Table of Contents
- [Basics](#basics)
- [Variables and Data Types](#variables-and-data-types)
- [Operators](#operators)
- [Input and Output](#input-and-output)
- [Loops](#loops)
- [Functions](#functions)
- [Arrays and Vectors](#arrays-and-vectors)
- [Structs and Classes](#structs-and-classes)
- [Pointers and References](#pointers-and-references)

---

## Cheat Sheet Contents
### Basics
Every C++ program starts with a `main()` function.  
You need to include headers (like `<iostream>`) to use input/output.
The program below prints text to the console.

```cpp
#include <iostream>
using namespace std;

int main() {
    cout << "Hello, World!" << endl;
    return 0;
}
```

____

### Variables and Data Types  
Variables are named storage for values.
C++ is statically typed, so you must declare the type of each variable before using it.
- `int` → whole numbers
- `double` → decimal numbers
- `char` → single characters
- `bool` → true/false values
- `string` → text

 ```cpp
int age = 16;
double pi = 3.14;
char grade = 'A';
bool isCoding = true;
string name = "Alex";
```


____


### Operators  
Operators perform calculations and comparisons.
- Arithmetic: `+`, `-`, `*`, `/`, `%`
- Comparison: `==`, `!=`, `<`, `>`, `<=`, `>=`
- Logical: `&&` (and), `||` (or), `!` (not)

```cpp
int a = 5, b = 2;

int sum = a + b;       // 7
int product = a * b;   // 10
bool result = (a > b); // true
```

____

### Input and Output
`cout` prints to the console, while `cin` reads input from the user.

```cpp
#include <iostream>
using namespace std;

int main() {
    int age;
    cout << "Enter your age: ";
    cin >> age;
    cout << "You are " << age << " years old." << endl;
}
```

____

### Loops 
Loops allow you to repeat code multiple times.
- `for` → when you know how many times to repeat
- `while` → repeats while a condition is true
- `do...while` → similar to `while`, but runs at least once

```cpp
// for loop
for (int i = 0; i < 3; i++) {
    cout << "i = " << i << endl;
}

// while loop
int n = 0;
while (n < 3) {
    cout << "n = " << n << endl;
    n++;
}
```
____

### Functions 
Functions are reusable blocks of code that perform a specific task.
They improve readability and reduce repetition.

```cpp
#include <iostream>
using namespace std;

int add(int x, int y) {
    return x + y;
}

int main() {
    cout << add(3, 4); // Output: 7
}
```

____

### Arrays and Vectors  
Arrays store multiple values of the same type with a fixed size.
Vectors (from `<vector>`) are dynamic arrays that can grow or shrink.

```cpp
#include <iostream>
#include <vector>
using namespace std;

int numbers[3] = {1, 2, 3};  // array

vector<int> values;          // vector
values.push_back(10);
values.push_back(20);

cout << values[0]; // prints 10
```

____

### Structs and Classes  
Structs and classes group related data (and in classes, also functions).
They are the foundation of object-oriented programming in C++.

```cpp
#include <iostream>
using namespace std;

struct Player {
    string name;
    int score;
};

class Car {
public:
    string brand;
    void drive() {
        cout << brand << " is driving" << endl;
    }
};

int main() {
    Player p = {"Alex", 100};
    cout << p.name << " scored " << p.score << endl;

    Car c;
    c.brand = "BMW";
    c.drive();
}
```

____

### Pointers and References
Pointers store the memory address of a variable.
References act as an alias (another name) for a variable.

```cpp
#include <iostream>
using namespace std;

int main() {
    int x = 10;

    int* ptr = &x;   // pointer to x
    int& ref = x;    // reference to x

    cout << *ptr << endl; // prints 10
    ref = 20;             // changes x to 20
    cout << x << endl;    // prints 20
}
```






