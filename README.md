# 🔧 Libft - Custom C Standard Library

[![C](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white)](https://en.wikipedia.org/wiki/C_(programming_language))
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Complete-brightgreen.svg)]()
[![Build](https://img.shields.io/badge/Build-Passing-success.svg)]()
[![Version](https://img.shields.io/badge/Version-1.0.0-blue.svg)]()

<div align="center">

# 🔧 Libft - 42 Custom C Library

> A comprehensive reimplementation of the C standard library functions, plus additional utilities, for the 42 curriculum.

**Master C fundamentals by building your own standard library!**

[![GitHub stars](https://img.shields.io/github/stars/yourusername/libft-42?style=social)](https://github.com/yourusername/libft-42/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/yourusername/libft-42?style=social)](https://github.com/yourusername/libft-42/network)
[![GitHub issues](https://img.shields.io/github/issues/yourusername/libft-42)](https://github.com/yourusername/libft-42/issues)

</div>

---

## 📚 Table of Contents

- [🎯 Overview](#-overview)
- [✨ Features](#-features)
- [🛠️ Installation](#️-installation)
- [🚀 Usage](#-usage)
- [📁 Project Structure](#-project-structure)
- [🛠️ Technologies Used](#️-technologies-used)
- [🧪 Testing](#-testing)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

## 🎯 Overview

Libft is a **custom implementation of the C standard library**. It includes essential string, memory, and list manipulation functions, as well as additional utilities. This project is a foundational part of the 42 curriculum and is designed to strengthen your understanding of C programming.

### 🎓 What You'll Learn
- **Memory management**: malloc, free, memset, memcpy, etc.
- **String manipulation**: strlen, strcpy, strcat, strchr, strstr, etc.
- **Character checks**: isalpha, isdigit, isalnum, isascii, isprint
- **List operations**: linked list creation, manipulation, and traversal
- **Custom utilities**: split, itoa, strmapi, etc.

## ✨ Features

### 🧰 Standard Library Functions
- ✅ String functions: strlen, strcpy, strcat, strdup, strchr, strstr, etc.
- ✅ Memory functions: memset, memcpy, memmove, memchr, memcmp, calloc, bzero
- ✅ Character checks: isalpha, isdigit, isalnum, isascii, isprint, toupper, tolower
- ✅ Conversion: atoi, itoa
- ✅ Output: putchar_fd, putstr_fd, putendl_fd, putnbr_fd

### 📝 Bonus Functions
- ✅ Linked list operations: lstnew, lstadd_front, lstadd_back, lstsize, lstlast, lstdelone, lstclear, lstiter, lstmap
- ✅ String utilities: split, strtrim, strjoin, substr, strmapi, striteri

### 🛡️ Robustness
- ✅ Error handling: Defensive programming and input validation
- ✅ Memory safety: Careful allocation and deallocation
- ✅ Comprehensive testing: Test files for all functions

## 🛠️ Installation

### Prerequisites
- **C compiler** (GCC or Clang)
- **Make** (GNU Make 4.0+)
- **Unix-like OS** (Linux, macOS)

### 🏗️ Building the Library
1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/libft-42.git
   cd libft-42
   ```
2. **Build the library**
   ```bash
   make
   ```

### 🔧 Make Commands
| Command      | Description                      |
|--------------|----------------------------------|
| `make`       | Builds the library (libft.a)     |
| `make clean` | Removes object files             |
| `make fclean`| Removes object files & library   |
| `make re`    | Rebuilds the library             |

## 🚀 Usage

### Linking with Your Project
1. **Include the header** in your source file:
   ```c
   #include "libft.h"
   ```
2. **Compile and link** with the library:
   ```bash
   gcc your_program.c -L. -lft -o your_program
   ```

### Example
```c
#include "libft.h"
#include <stdio.h>

int main(void) {
    char *s = ft_strdup("Hello, world!");
    printf("%s\n", s);
    free(s);
    return 0;
}
```

## 📁 Project Structure
```
libft-42/
├── ft_*.c            # C function implementations
├── libft.h           # Header file
├── Makefile          # Build configuration
├── README.md         # This file
```

## 🛠️ Technologies Used
### Programming Languages
![C](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white)

### Build Tools
![Make](https://img.shields.io/badge/Make-000000?style=for-the-badge&logo=gnu&logoColor=white)
![GCC](https://img.shields.io/badge/GCC-000000?style=for-the-badge&logo=gnu&logoColor=white)

### Development Tools
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white)

## 🧪 Testing
### Manual Testing
1. **Compile test files**
   ```bash
   gcc -Wall -Wextra -Werror test_ft_strlen.c libft.a -o test_strlen
   ./test_strlen
   ```
2. **Use provided test suites** or your own test files.

### Testing Tools
- [42Tester](https://github.com/Mazoise/42TESTERS-LIBFT)
- [libft-unit-test](https://github.com/alelievr/libft-unit-test)
- [libft-war-machine](https://github.com/y3ll0w42/libft-war-machine)

## 🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

### How to Contribute
1. **Fork the repository**
   ```bash
   git clone https://github.com/yourusername/libft-42.git
   ```
2. **Create your feature branch**
   ```bash
   git checkout -b feature/AmazingFeature
   ```
3. **Make your changes**
   - Follow the existing code style
   - Add tests for new features
   - Update documentation as needed
4. **Commit your changes**
   ```bash
   git commit -m 'Add some AmazingFeature'
   ```
5. **Push to the branch**
   ```bash
   git push origin feature/AmazingFeature
   ```
6. **Open a Pull Request**

### Contribution Guidelines
- Follow the existing code style and conventions
- Add tests for new features
- Update documentation as needed
- Ensure the library compiles without warnings

## 📄 License
This project is part of the 42 School curriculum. The code is written for educational purposes.

---

<div align="center">

**Made with ❤️ and lots of ☕**

*Master C fundamentals by building your own standard library!*

[![GitHub stars](https://img.shields.io/github/stars/yourusername/libft-42?style=social)](https://github.com/yourusername/libft-42/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/yourusername/libft-42?style=social)](https://github.com/yourusername/libft-42/network)
[![GitHub issues](https://img.shields.io/github/issues/yourusername/libft-42)](https://github.com/yourusername/libft-42/issues)

**Author**: [Your Name]  
**School**: 42 School  
**Project**: Libft  
**Last updated**: December 2024

</div> 