---
layout: default
title: Lecture 4
---

🇸🇦 [Arabic](https://translate.google.com/translate?hl=ar&sl=en&u=https://okhalifa-official.github.io/CP-L1_PTA/Lec4) 🇫🇷 [French](https://translate.google.com/translate?hl=fr&sl=en&u=https://okhalifa-official.github.io/CP-L1_PTA/Lec4) 🇪🇸 [Spanish](https://translate.google.com/translate?hl=es&sl=en&u=https://okhalifa-official.github.io/CP-L1_PTA/Lec4) 🇩🇪 [German](https://translate.google.com/translate?hl=de&sl=en&u=https://okhalifa-official.github.io/CP-L1_PTA/Lec4)


# Char Arrays & Strings

## Char Arrays

### I/O Operations
* You can input and output char arrays using standard input/output functions.
* For example, reading a char array as a string using `cin` and printing it with `cout`.
```cpp
char str;
cin >> str; // Input a string into char array
cout << str << endl; // Output the string
```

### Accessing Elements
* Char arrays are accessed using their index starting from 0, similar to other arrays.
* You can access or modify individual characters by specifying their index.
```cpp
char arr = {'H', 'e', 'l', 'l', 'o'};
cout << arr; // Output: e
arr = 'a'; // Modify last element
```

## Strings

### Null Terminator

* When using `cin` to read input into a character array, it stops reading at the first space and automatically appends a null terminator (`'\0'`) to mark the end of the string.

* A null terminator is a special character (`'\0'`) that marks the end of a C-style string.

* It's automatically added at the end of string literals in C-style strings.

* Important when using character arrays instead of `string` class.

* Without the null terminator, functions like `strlen()` and `cout` may read garbage values beyond the intended end.

* Example:

  ```cpp
  char name[] = "Omar";
  // Actually stored as: ['O', 'm', 'a', 'r', '\0']
  ```

### Operations on Strings

* `getline()` reads an entire line including spaces until a newline is encountered.

* Useful when reading full sentences or names with spaces.

* Syntax: `getline(cin, variable);`

* Example:

  ```cpp
  #include <iostream>
  #include <string>
  using namespace std;

  string sentence;
  getline(cin, sentence);
  cout << "You entered: " << sentence;
  ```

* Strings are sequences of characters.

* Declare: `string name = "Omar";`

* Combine: `s1 + s2`

* Length: `s.length()` or `s.size()`

* Access characters with `s[i]`

* Loop through:

  ```cpp
  for (char c : s) {
      cout << c << " "; // print all chars in string
  }
  ```

### Casting Digits from Characters

* Convert character digits like `'5'` to int:

  ```cpp
  char ch = '5';
  int digit = ch - '0'; // digit = 5
  ```

### Converting String to Integer (stoi)

* Use `stoi()` to convert an entire string to an integer.
* Only works with numeric strings like "123".
* Defined in `<string>`.
* Example:

  ```cpp
  #include <string>
  string numStr = "456";
  int num = stoi(numStr); // num = 456
  ```

  ```cpp
  char ch = '5';
  int digit = ch - '0'; // digit = 5
  ```

---

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
<br>

"The only way to learn a new programming language is by writing programs in it."
— Dennis Ritchie
<br>
<br>

---

<br>

© 2025 Pathline Training Academy | Made with 💙 by Omar Khalifa  
[Back to Top](#top)
