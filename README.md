# SyntaX (bettersyntax.h) 🚀

**SyntaX** is a lightweight, header-only C++ library designed to bring the **simplicity of Python's syntax** together with the **raw performance of C++**. 

Are you tired of complex C++ boilerplate code for simple tasks? **SyntaX** allows you to write cleaner, more readable code without sacrificing speed. It is the perfect bridge for developers who love Python's ease of use but need C++'s execution power.

---

## 🌟 Key Features

* **Python-like Syntax:** Familiar functions like `print()`, `input()`, and `randint()`.
* **Cross-Platform:** Built-in support for **Windows, Linux, and macOS** using native APIs.
* **Header-Only:** No complex installation or linking required. Just drop `bettersyntax.h` into your project.
* **Legacy Compiler Support:** Specifically optimized to work with **MinGW 6** and older environments where modern `std::thread` or `std::chrono` might be unstable.
* **Memory Efficient:** Uses constant reference passing and optimized C++ streams for maximum performance.

---

## 🛠️ Usage & Examples

To keep this documentation clean, we have provided a dedicated example file. You can find comprehensive usage examples covering:

* **Simplified I/O** (print and input)
* **File Operations** (read/write/append)
* **Vector & Math Helpers** (contains, sum, average, factorial)
* **System Utilities** (clear screen and sleep)

👉 **Check out [samples.cpp](./samples.cpp) for ready-to-use code snippets!**

---

## 📂 Installation

1. Download the **bettersyntax.h** file from this repository.
2. Place it in your project's include directory or the root folder.
3. Add **#include "bettersyntax.h"** at the top of your source code.
4. Use the **bettersyntax::** prefix or add **using namespace bettersyntax;** to start coding!

## 🚀 Advanced Installation (System-wide)

If you want to use **SyntaX** globally on your computer like `<iostream>`, follow these steps:

1. Locate your compiler's include directory (e.g., `C:\MinGW\include`).
2. Copy `bettersyntax.h` into that folder.
3. (Optional) Rename it to `bettersyntax` (without the `.h`) for a cleaner look.
4. Now you can include it in any project using:
   ```cpp
   #include <bettersyntax>

## 💻 Technical Details
The library is safely wrapped in the **bettersyntax** namespace to prevent name collisions with the standard library (`std`) or other third-party tools. It uses preprocessor directives to ensure stability across different Operating Systems.

---

## Development Comparison

| Feature | Standard C++ (STL) | **SyntaX for C++** (`bettersyntax`) |
| :--- | :--- | :--- |
| **Output** | `std::cout << x << " " << y << std::endl;` | `print(x, y);` |
| **User Input** | `std::string s; std::getline(std::cin, s);` | `string s = input("Name: ");` |
| **Random Number** | `min + (std::rand() % (max - min + 1));` | `randint(min, max);` |
| **Sleep/Wait** | `#ifdef _WIN32 Sleep(1000); #else usleep...` | `sleep(1.0);` |
| **File Reading** | `std::ifstream`, `stringstream`, `rdbuf()...` | `read_file("data.txt");` |
| **Vector Search** | `std::find(v.begin(), v.end(), x) != v.end()` | `contains(vec, x);` |
| **Math (Sqrt)** | `std::sqrt(val);` | `square_root(val);` |
| **Clear Screen** | `system("cls");` or `system("clear");` | `clear();` |

---

### 👨‍💻 Programmer
**hypernova-developer**
