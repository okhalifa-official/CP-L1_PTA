---
layout: default
title: Lecture 5
---

🇸🇦 [Arabic](https://translate.google.com/translate?hl=ar&sl=en&u=https://okhalifa-official.github.io/CP-L1_PTA/Lec5) 🇫🇷 [French](https://translate.google.com/translate?hl=fr&sl=en&u=https://okhalifa-official.github.io/CP-L1_PTA/Lec5) 🇪🇸 [Spanish](https://translate.google.com/translate?hl=es&sl=en&u=https://okhalifa-official.github.io/CP-L1_PTA/Lec5) 🇩🇪 [German](https://translate.google.com/translate?hl=de&sl=en&u=https://okhalifa-official.github.io/CP-L1_PTA/Lec5)


# Functions & Built-in Functions

## Functions

### Function Implementation

* Reusable blocks of code that perform specific tasks.
* Helps make your code cleaner, modular, and easier to debug.
* A function has a return type, a name, parameters (optional), and a body.
* Example:

  ```cpp
  int add(int a, int b) {
      return a + b; // returns the sum of a and b to where the function was called
  }
  ```

### return Statement

* `return` is used to send a value back from the function to where it was called.
* Once `return` is executed, the function ends immediately.
* If the function has a return type (like `int`), you must return a value of that type.
* Example:

  ````cpp
  int square(int x) {
      return x * x;
  }
  ````
* Define functions to organize your program better.
* Example:

  ```cpp
  int add(int a, int b) {
      return a + b;
  }
  ```

### Function Calling

* Call a function by its name and pass arguments:

  ```cpp
  int result = add(3, 4); // Output: 7
  ```

### Passing by Value
When you **pass by value**, a **copy** of the variable’s value is sent to the function.  
This means the function works on its **own copy**, not the original variable.

- Changes made inside the function **do not affect** the original variable.
- Safe, because the original data stays untouched.
- Slightly slower for large data, since it creates a copy.

### Example (C++)

```cpp
#include <iostream>
using namespace std;

void changeValue(int x) {
    x = 100;  // only changes the local copy
}

int main() {
    int a = 5;
    changeValue(a);
    cout << a;  // prints 5 (unchanged)
}
```

### Passing by Reference
When you **pass by reference**, the function gets a **direct link (alias)** to the original variable.  
This means the function can **change the actual variable**, not just a copy.

- Changes inside the function **do affect** the original variable.
- Faster for large data, since no copy is made.
- Must be used carefully to avoid unintended changes.

### Example (C++)

```cpp
#include <iostream>
using namespace std;

void changeValue(int &x) {
    x = 100;  // modifies the original variable
}

int main() {
    int a = 5;
    changeValue(a);
    cout << a;  // prints 100 (changed)
}
```

---

## Built-in Functions

### cmath Library

* Math functions like `sqrt()`, `pow()`, `abs()`, `ceil()`, `floor()`, `round()`, etc.
* Include the library:

  ```cpp
  #include <cmath>
  cout << sqrt(16); // Output: 4
  cout << pow(5,3); // Output: 125
  cout << abs(-2); // Output: 2
  cout << ceil(2.1); // Output: 3
  cout << floor(4.8); // Output: 4
  cout << round(7.3) << round(7.8); // Output: 7 8
  ```

### algorithm Library

* Useful for sorting, finding max/min, reversing arrays, etc.
* Common functions:

  * `sort(arr, arr + n)`
  * `reverse(arr, arr + n)`
  * `max(a,b)`, `min(a,b)`
  * `find(arr, arr + n, target)`
* Example:

  ```cpp
  #include <algorithm>
  int arr[] = {3, 1, 4};
  sort(arr, arr + 3);
  ```

### cctype Library

* Useful for checking and converting characters.
* Include the library:

  ```cpp
  #include <cctype>
  ```
* Common functions:

  * `isdigit(c)` → checks if `c` is a digit.
  * `isalpha(c)` → checks if `c` is a letter.
  * `islower(c)` → checks if `c` is lowercase.
  * `isupper(c)` → checks if `c` is uppercase.
  * `tolower(c)` → converts to lowercase.
  * `toupper(c)` → converts to uppercase.
* Example:

  ```cpp
  char ch = 'A';
  if (isupper(ch)) cout << tolower(ch); // Output: a
  ```

Find more functions and documentation on [cppreference.com](https://en.cppreference.com)

<br>

"The only way to learn a new programming language is by writing programs in it."
— Dennis Ritchie
<br>
<br>

---

<br>

© 2025 Pathline Training Academy | Made with 💙 by Omar Khalifa  
[Back to Top](#top)
