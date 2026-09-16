# 🚀 Utility Library in C++ (OOP)

A reusable C++ Utility Library that provides a collection of helper functions for random data generation, array manipulation, value swapping, text encryption, formatting, and number conversion.

The project is implemented using a static utility class, clsUtil, allowing developers to access the provided functions directly without creating objects.

This project demonstrates practical applications of Object-Oriented Programming (OOP), function overloading, code reuse, modular programming, and utility library design.

---

## 📚 Background


The main goal of the project is to understand how reusable utility/helper libraries can be designed and implemented in C++ and how common programming operations can be organized into a single reusable class.

---

## 🧠 Key Concepts Practiced

- Object-Oriented Programming (OOP)
- Static Classes
- Static Member Functions
- Function Overloading
- References and Pass-by-Reference
- Code Reusability
- Modular Programming
- Random Number Generation
- Arrays
- Strings
- Recursion
- Basic Encryption
- Clean Code Practices

---

## ⚙️ Library Features

### 🎲 Random Utilities

The library provides several functions for generating random data.

Features include:

- Generate random numbers within a specific range
- Generate random characters
- Generate random words
- Generate random keys
- Generate multiple keys

Example:

GHTR-YUOP-ABCD-WXYZ
P9QW-RT56-ABCD-XYZ1

Example usage:

    cout << clsUtil::RandomNumber(1, 10) << endl;
    cout << clsUtil::GetRandomCharacter(clsUtil::CapitalLetter) << endl;
    cout << clsUtil::GenerateWord(clsUtil::MixChars, 8) << endl;
    cout << clsUtil::GenerateKey(clsUtil::MixChars) << endl;

---

## 📦 Array Utilities

The library provides helper functions for working with arrays.

Features include:

- Fill arrays with random numbers
- Fill arrays with random words
- Fill arrays with random keys
- Shuffle array elements randomly

These functions demonstrate how utility methods can simplify repetitive programming tasks.

---

## 🔄 Swap Functions

The library provides overloaded Swap() functions for different data types.

Supported types include:

- int
- double
- bool
- char
- string
- clsDate

Example:

    int x = 10;
    int y = 20;

    clsUtil::Swap(x, y);

    cout << x << " " << y << endl;

Output:

    20 10

The project demonstrates Function Overloading, where multiple functions can have the same name while accepting different parameter types.

---

## 🔐 Text Encryption

The library includes a simple Caesar-style encryption and decryption system.

Features include:

- Encrypt text using a numeric key
- Decrypt encrypted text
- Preserve the original text after decryption

Example:

Before:
ABDELMOUMEN BENHADDAD

Encrypted:
Oqjcoogf Cdw-Jcfjqwpf

Decrypted:
ABDELMOUMEN BENHADDAD

Example usage:

    string Text = "ABDELMOUMEN BENHADDAD";

    string Encrypted = clsUtil::EncryptText(Text, 2);
    string Decrypted = clsUtil::DecryptText(Encrypted, 2);

    cout << "Before: " << Text << endl;
    cout << "Encrypted: " << Encrypted << endl;
    cout << "Decrypted: " << Decrypted << endl;

Note: This encryption implementation is intended for learning purposes and is not suitable for securing sensitive information in real-world applications.

---

## 🧾 Number to Text Conversion

The library can convert numerical values into their English text representation.

Example:

1250

becomes:

One Thousand Two Hundred Fifty

This feature demonstrates:

- Recursive problem solving
- Conditional logic
- Number decomposition
- String manipulation

---

## 🔑 Static Utility Class

The main functionality of the project is organized inside the clsUtil class.

Example:

    clsUtil::RandomNumber(1, 10);

Instead of creating an object:

    clsUtil Util;

The functions can be accessed directly through the class name.

This is possible because the utility functions are implemented as static member functions.

The design is useful for functions that do not need to store object-specific data.

---

## 🏗️ Function Overloading

The project also demonstrates function overloading.

For example, Swap() can work with different data types:

    clsUtil::Swap(intA, intB);
    clsUtil::Swap(doubleA, doubleB);
    clsUtil::Swap(charA, charB);
    clsUtil::Swap(stringA, stringB);

The compiler determines which version of the function should be called based on the arguments provided.

---

## 📂 Project Structure

    Utility-Library-Cpp/
    │
    ├── clsUtil.h
    ├── clsDate.h
    ├── main.cpp
    └── README.md

### clsUtil.h

Contains the utility class and its helper functions.

### clsDate.h

Contains the clsDate class used by some utility functions, including the overloaded Swap() function.

### main.cpp

Contains examples demonstrating how to use the utility library.

---

## 💻 Usage Example

    #include <iostream>
    #include "clsUtil.h"

    using namespace std;

    int main()
    {
        clsUtil::Srand();

        cout << clsUtil::RandomNumber(1, 10) << endl;

        cout << clsUtil::GetRandomCharacter(clsUtil::CapitalLetter) << endl;

        cout << clsUtil::GenerateWord(clsUtil::MixChars, 8) << endl;

        cout << clsUtil::GenerateKey(clsUtil::MixChars) << endl;

        clsUtil::GenerateKeys(3, clsUtil::MixChars);

        int x = 10;
        int y = 20;

        clsUtil::Swap(x, y);

        cout << x << " " << y << endl;

        string Text = "ABDELMOUMEN BENHADDAD";

        string Encrypted = clsUtil::EncryptText(Text, 2);
        string Decrypted = clsUtil::DecryptText(Encrypted, 2);

        cout << "Before: " << Text << endl;
        cout << "Encrypted: " << Encrypted << endl;
        cout << "Decrypted: " << Decrypted << endl;

        return 0;
    }

---

## 🛠️ Technologies Used

- C++
- Object-Oriented Programming
- Standard C++ Library
- Visual Studio / C++ Compiler

---

## 📈 Learning Outcomes

Through this project, I strengthened my understanding of:

- Designing reusable C++ classes
- Static classes and static member functions
- Function overloading
- Passing variables by reference
- Random data generation
- Array manipulation
- String processing
- Recursion
- Basic encryption algorithms
- Modular and reusable code
- Organizing a C++ project for maintainability

The project helped me move from writing individual programs toward designing reusable components and libraries that can be integrated into other applications.

---

## 🎯 Purpose of the Project

The purpose of this project is educational.

It was created to practice C++ and OOP concepts through a practical project rather than isolated programming exercises.

The utility library can also serve as a reusable component for future C++ projects.

---

## 👨‍🏫 Acknowledgments


---

## 👨‍💻 Author

Abdelmoumen Benhaddad

Computer Science Student | C++ | OOP | Algorithms & Data Structures
