# 📚 Libft - 42 School C Library

[![42](https://img.shields.io/badge/42-Libft-blue)](https://42.fr)
[![C](https://img.shields.io/badge/C-99%20Standard-green)](https://en.wikipedia.org/wiki/C99)
[![License](https://img.shields.io/badge/License-MIT-yellow)](LICENSE)
[![Build Status](https://img.shields.io/badge/Build-Passing-brightgreen)]()

A comprehensive C library implementing standard library functions and additional utilities, created as part of the 42 school curriculum.

## 🎯 Overview

Libft is a collection of 44 C functions that reimplements many standard C library functions, plus additional utility functions and a complete linked list implementation. This project serves as the foundation for future 42 school projects.

## 📋 Table of Contents

- [Features](#-features)
- [Installation](#-installation)
- [Usage](#-usage)
- [Functions](#-functions)
- [Examples](#-examples)
- [Testing](#-testing)
- [Contributing](#-contributing)
- [License](#-license)

## ✨ Features

- **44 Functions**: 35 core functions + 9 bonus linked list functions
- **Memory Safe**: Proper memory allocation and deallocation
- **42 Compliant**: Follows 42 school coding standards
- **Well Documented**: Clear function descriptions and usage
- **Modular Design**: Easy to integrate into other projects

## 🚀 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/libft-42.git
   cd libft-42
   ```

2. **Compile the library**
   ```bash
   # Compile core functions only
   make
   
   # Compile with bonus functions (linked lists)
   make bonus
   ```

3. **Clean build files** (optional)
   ```bash
   make clean      # Remove object files
   make fclean     # Remove object files and library
   ```

## 📖 Usage

### Basic Usage

```c
#include "libft.h"

int main(void)
{
    char *str = "Hello, World!";
    int len = ft_strlen(str);
    
    ft_putstr_fd("Length: ", 1);
    ft_putnbr_fd(len, 1);
    ft_putchar_fd('\n', 1);
    
    return (0);
}
```

### Linking with Your Project

```bash
# Compile your program with libft
gcc -Wall -Wextra -Werror your_program.c libft.a -o your_program
```

## 🔧 Functions

### Character Functions
| Function | Description |
|----------|-------------|
| `ft_isalpha` | Check if character is alphabetic |
| `ft_isdigit` | Check if character is a digit |
| `ft_isalnum` | Check if character is alphanumeric |
| `ft_isascii` | Check if character is ASCII |
| `ft_isprint` | Check if character is printable |
| `ft_toupper` | Convert character to uppercase |
| `ft_tolower` | Convert character to lowercase |

### String Functions
| Function | Description |
|----------|-------------|
| `ft_strlen` | Calculate string length |
| `ft_strchr` | Find first occurrence of character |
| `ft_strrchr` | Find last occurrence of character |
| `ft_strncmp` | Compare strings up to n characters |
| `ft_strnstr` | Find substring in string |
| `ft_strdup` | Duplicate string |
| `ft_strlcpy` | Copy string with size limit |
| `ft_strlcat` | Concatenate strings with size limit |
| `ft_strjoin` | Join two strings |
| `ft_strtrim` | Remove characters from start/end |
| `ft_substr` | Extract substring |
| `ft_split` | Split string by delimiter |
| `ft_strmapi` | Apply function to each character |
| `ft_striteri` | Apply function to each character with index |

### Memory Functions
| Function | Description |
|----------|-------------|
| `ft_memset` | Set memory to value |
| `ft_bzero` | Set memory to zero |
| `ft_memcpy` | Copy memory |
| `ft_memmove` | Move memory (handles overlap) |
| `ft_memchr` | Find character in memory |
| `ft_memcmp` | Compare memory |
| `ft_calloc` | Allocate and zero memory |

### Conversion Functions
| Function | Description |
|----------|-------------|
| `ft_atoi` | Convert string to integer |
| `ft_itoa` | Convert integer to string |

### File Descriptor Functions
| Function | Description |
|----------|-------------|
| `ft_putchar_fd` | Write character to file descriptor |
| `ft_putstr_fd` | Write string to file descriptor |
| `ft_putendl_fd` | Write string + newline to file descriptor |
| `ft_putnbr_fd` | Write number to file descriptor |

### Linked List Functions (Bonus)
| Function | Description |
|----------|-------------|
| `ft_lstnew` | Create new list element |
| `ft_lstadd_front` | Add element to front of list |
| `ft_lstadd_back` | Add element to back of list |
| `ft_lstsize` | Count list elements |
| `ft_lstlast` | Get last element |
| `ft_lstdelone` | Delete single element |
| `ft_lstclear` | Delete entire list |
| `ft_lstiter` | Apply function to each element |
| `ft_lstmap` | Create new list with transformed elements |

## 💡 Examples

### String Manipulation
```c
char *str = "  Hello World  ";
char *trimmed = ft_strtrim(str, " ");
// Result: "Hello World"

char **words = ft_split("hello,world,test", ',');
// Result: ["hello", "world", "test", NULL]
```

### Linked List Usage
```c
t_list *list = ft_lstnew("first");
ft_lstadd_back(&list, ft_lstnew("second"));
ft_lstadd_back(&list, ft_lstnew("third"));

int size = ft_lstsize(list); // Returns 3
```

### Memory Management
```c
char *str = ft_calloc(10, sizeof(char));
// Allocates and zeros 10 bytes

ft_memset(str, 'A', 5);
// Sets first 5 bytes to 'A'
```

## 🧪 Testing

The library includes comprehensive testing. You can test individual functions or run the full test suite:

```bash
# Test specific function
gcc -Wall -Wextra -Werror test_strlen.c libft.a -o test_strlen
./test_strlen

# Run all tests (if test suite is available)
make test
```

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Coding Standards

- Follow 42 school coding norms
- Use proper header formatting
- Include error handling
- Write clear comments
- Test all functions thoroughly

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Your Name**
- GitHub: [@yourusername](https://github.com/yourusername)
- 42 School: [@your42username](https://42.fr)

## 🙏 Acknowledgments

- 42 School for the project requirements
- The C programming community
- All contributors and reviewers

---

<div align="center">
  <p>Made with ❤️ for 42 School</p>
  <p>⭐ Star this repository if you found it helpful!</p>
</div>