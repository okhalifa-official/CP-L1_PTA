---
layout: default
title: Lecture 2
---

🇸🇦 [Arabic](https://translate.google.com/translate?hl=ar&sl=en&u=https://okhalifa-official.github.io/CP-L1_PTA/Lec2) 🇫🇷 [French](https://translate.google.com/translate?hl=fr&sl=en&u=https://okhalifa-official.github.io/CP-L1_PTA/Lec2) 🇪🇸 [Spanish](https://translate.google.com/translate?hl=es&sl=en&u=https://okhalifa-official.github.io/CP-L1_PTA/Lec2) 🇩🇪 [German](https://translate.google.com/translate?hl=de&sl=en&u=https://okhalifa-official.github.io/CP-L1_PTA/Lec2)



# Control Program Flow

### Remember*

Booleans store either `true` or `false`.

```cpp
bool isEven = (num % 2 == 0);
```

---

## If Statements

If something is true, do this.

```cpp
if (x > 10) {
   cout << "Greater than 10";
}
```

If something is true, do this.
If it's not true, do that.
```cpp
if (x > 10) {
    cout << "Greater than 10";
} else {
    cout << "10 or less";
}
```

If true, do plan A.
else, do plan B.
else, do plan C.
...
```cpp
if (x > 10) {
    cout << "Greater than 10";
} else if (x == 10) {
    cout << "Exactly 10";
} else {
    cout << "Less than 10";
}

```

---

### Nested Ifs

You can place if-statements inside others to check multiple conditions.

```cpp
if (x > 0) {
   if (x < 10) {
      cout << "Between 1 and 9";
   }
}
```

---

## Loops

Loops help you **repeat** tasks without rewriting code.

### For Loop

Used when you know how many times to repeat.

```cpp
for (int i = 0; i < 5; i++) {
   cout << i << " ";
}
```

---

### While Loop

Repeats while a condition is true.

```cpp
int i = 0;
while (i < 5) {
   cout << i << " ";
   i++;
}
```

---

### Infinite Loops

Be careful! If your condition **never becomes false**, your loop will run forever.

```cpp
while (true) {
   // This never stops
}
```

Don't forget to break out of the infinite loops.
```cpp
while (true) {
   // Stop when a condition is true
   if(condition){
        break;
   }
}
```

---

### Problems
#### print all even numbers 1 -> 100
```cpp
for (int i=2; i<=100; i+=2){
   cout<< i << endl;
}
```
#### print all odd numbers 1 -> 100
```cpp
for (int i=1; i<=100; i+=2){
   cout<< i << endl;
}
```
#### print all numbers divisible by 3
```cpp
for (int i=1; i<=100; i++){
   if(i % 3 == 0)
      cout<< i << endl;
}
for (int i=3; i<=100; i+=3){
   cout<< i << endl;
}
```
#### print all numbers divisible by 3 or 5
```cpp
for(int i=1; i<=100; i++){
   if(i % 3 == 0 || i % 5 == 0){
      cout << i << endl;
   }
}
```
#### print all numbers divisible by 3 and 5 and 7
```cpp
for(int i=3*5*7; i<=1000; i+=3*5*7){
   cout << i << endl;
}
```

🌱 **Small progress each day adds up to big results.**
Keep going — consistency is your superpower!
<br>
<br>

---

<br>

© 2025 Pathline Training Academy | Made with 💙 by Omar Khalifa  
[Back to Top](#top)
