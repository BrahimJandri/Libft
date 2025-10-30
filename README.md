# Libft - Your First Own Library

![Libft](libft.png)

## 📖 Table of Contents
- [About](#about)
- [Functions](#functions)
  - [Part 1 - Libc Functions](#part-1---libc-functions)
  - [Part 2 - Additional Functions](#part-2---additional-functions)
- [Installation](#installation)
- [Usage](#usage)
- [Compilation](#compilation)
- [Author](#author)

## About

**Libft** is a custom C library that reimplements many of the standard C library functions. This project is part of the 42 School curriculum and serves as a foundation for future C projects.

C programming can be very tedious when one doesn't have access to the highly useful standard functions. This project is about understanding the way these functions work, implementing and learning to use them. You will create your own library that will be helpful in your next C school assignments.

## Functions

### Part 1 - Libc Functions

These functions are reimplementations of standard C library functions:

#### Character Checks & Conversions
- `ft_isalpha` - Check if character is alphabetic
- `ft_isdigit` - Check if character is a digit
- `ft_isalnum` - Check if character is alphanumeric
- `ft_isascii` - Check if character is ASCII
- `ft_isprint` - Check if character is printable
- `ft_toupper` - Convert character to uppercase
- `ft_tolower` - Convert character to lowercase

#### String Functions
- `ft_strlen` - Calculate string length
- `ft_strchr` - Locate character in string
- `ft_strrchr` - Locate character in string (from end)
- `ft_strncmp` - Compare strings (n bytes)
- `ft_strnstr` - Locate substring in string
- `ft_strlcpy` - Copy string with size limit
- `ft_strlcat` - Concatenate string with size limit
- `ft_strdup` - Duplicate string

#### Memory Functions
- `ft_memset` - Fill memory with constant byte
- `ft_bzero` - Zero out memory
- `ft_memcpy` - Copy memory area
- `ft_memmove` - Copy memory area (handles overlap)
- `ft_memchr` - Scan memory for character
- `ft_memcmp` - Compare memory areas
- `ft_calloc` - Allocate and zero memory

#### Conversion Functions
- `ft_atoi` - Convert string to integer

### Part 2 - Additional Functions

These are additional utility functions not present in the standard C library:

#### String Manipulation
- `ft_substr` - Extract substring from string
- `ft_strjoin` - Concatenate two strings
- `ft_strtrim` - Trim characters from start and end of string
- `ft_split` - Split string by delimiter into array
- `ft_strmapi` - Apply function to each character (with index)
- `ft_striteri` - Apply function to each character (void)

#### Conversion Functions
- `ft_itoa` - Convert integer to string

#### Output Functions
- `ft_putchar_fd` - Output character to file descriptor
- `ft_putstr_fd` - Output string to file descriptor
- `ft_putendl_fd` - Output string with newline to file descriptor
- `ft_putnbr_fd` - Output number to file descriptor

## Installation

Clone the repository:

```bash
git clone https://github.com/BrahimJandri/Libft.git
cd Libft
```

## Usage

Include the header in your C file:

```c
#include "libft.h"
```

Example:

```c
#include "libft.h"
#include <stdio.h>

int main(void)
{
    char *str = "Hello, World!";
    
    printf("Length: %zu\n", ft_strlen(str));
    printf("Uppercase: %c\n", ft_toupper('a'));
    
    return 0;
}
```

## Compilation

Compile the library:

```bash
make        # Compile the library
make clean  # Remove object files
make fclean # Remove object files and library
make re     # Recompile everything
```

This will create `libft.a` which you can link with your projects:

```bash
cc -Wall -Wextra -Werror your_file.c libft.a -o your_program
```

## Author

**Brahim Jandri** (bjandri)
- 42 School Student
- GitHub: [@BrahimJandri](https://github.com/BrahimJandri)
