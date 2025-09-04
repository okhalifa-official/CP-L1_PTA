---
layout: default
title: Lecture 3
---

🇸🇦 [Arabic](https://translate.google.com/translate?hl=ar&sl=en&u=https://okhalifa-official.github.io/CP-L1_PTA/Lec3) 🇫🇷 [French](https://translate.google.com/translate?hl=fr&sl=en&u=https://okhalifa-official.github.io/CP-L1_PTA/Lec3) 🇪🇸 [Spanish](https://translate.google.com/translate?hl=es&sl=en&u=https://okhalifa-official.github.io/CP-L1_PTA/Lec3) 🇩🇪 [German](https://translate.google.com/translate?hl=de&sl=en&u=https://okhalifa-official.github.io/CP-L1_PTA/Lec3)


# Loops
## Nested Loops
A loop inside another loop - often used for working with grids or pairs.

```cpp
for (int i = 0; i < 3; i++) {
   for (int j = 0; j < 3; j++) {
      cout << "(" << i << "," << j << ") ";
   }
}
```

# Arrays

## 1D Arrays

* A list of elements stored in a single row.
* All elements must be of the same data type (like `int`, `char`, etc.).
* You access elements using their index starting from **0**.
* Example:

  ```cpp
  int arr[5] = {10, 20, 30, 40, 50};
  cout << arr[2]; // Output: 30
  ```

## 2D Arrays

* Arrays arranged in rows and columns (like a table).
* Access elements using two indices: `arr[row][col]`
* Example:

  ```cpp
  int matrix[2][3] = {
      {1, 2, 3},
      {4, 5, 6}
  };
  cout << matrix[1][2]; // Output: 6
  ```

---

<br>

"The only way to learn a new programming language is by writing programs in it."
— Dennis Ritchie
<br>
<br>

---

<br>

© 2025 Pathline Training Academy | Made with 💙 by Omar Khalifa  
[Back to Top](#top)
