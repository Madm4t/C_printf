# C_printf
[![License](https://img.shields.io/badge/license-Unlicense-blue)](/LICENSE)

A reimplementation of the standard C `printf()` function.

## Table of Contents

- [About](#about)  
- [Features](#features)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Examples](#examples)  

## About

`C_printf` is a custom implementation of the standard C `printf()` function.  
This project was developed as part of the 42 School curriculum, enforcing strict coding norms and limitations to strengthen your understanding of variadic functions, formatting, and low-level string handling in C.

## Features

- Supports the following conversion specifiers:  
  - Characters: `%c`  
  - Strings: `%s`  
  - Pointers: `%p`  
  - Integers: `%d`, `%i`, `%u`  
  - Hexadecimal: `%x`, `%X`  
  - Literal percent sign: `%%`  
- 100% Norm-compliant:  
  - No forbidden standard functions  
  - Max 25 lines per function  
  - 80-column width limit  
  - No more than 4 functions per file  
  - Max 4 parameters per function  
- Thoroughly tested on edge cases (e.g., `NULL` pointers, zero values, large numbers).

## Installation

1. **Clone the repo**  
   ```bash
   git clone https://github.com/Madm4t/C-printf.git
   cd C-printf
2. Build the library
   ```bash
   make
This will produce libftprintf.a

## Usage

1. Include the header in your source file:
   ```bash
   #include "ft_printf.h"
2. Compile and link agians the library e.g.:
   ```bash
   gcc -Wall -Wextra -Werror -I. main.c -L. -lftprintf -o my_app
3. Callyour new ft_printf function just like the standard one:
   ```bash
   ft_printf("Hello, %s! You have %d new messages.\n", username, message_count);

Example main.c:
   ```bash
#include "ft_printf.h"

int main(void)
{
    int   n = 42;
    char *str = "world";
    ft_printf("Hello, %s! The answer is %d (hex: %#x)\n", str, n, n);
    return 0;
}


