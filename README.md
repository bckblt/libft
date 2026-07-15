# libft

A custom C standard library built from scratch as part of the 42 School curriculum. `libft` re-implements a set of essential libc functions and adds several custom utility functions, forming the foundation used in later 42 projects (`get_next_line`, `printf`, `minishell`, etc.).

## About

The goal of this project is to get comfortable with C by rebuilding core functions found in `<string.h>`, `<ctype.h>`, `<stdlib.h>`, and `<unistd.h>`, while also writing additional helper functions (string manipulation, memory allocation, and file-descriptor output) that are reused throughout the rest of the 42 curriculum.

## Compilation

```bash
make        # builds libft.a
make clean  # removes object files
make fclean # removes object files and the library
make re     # rebuilds everything from scratch
```

Include it in your project with:

```c
#include "libft.h"
```

and link it during compilation:

```bash
cc your_program.c -L. -lft -o your_program
```

## Functions

### Libc re-implementations
| Function | Description |
|---|---|
| `ft_isalpha` | Checks for an alphabetic character |
| `ft_isdigit` | Checks for a digit (0-9) |
| `ft_isalnum` | Checks for an alphanumeric character |
| `ft_isascii` | Checks for an ASCII character |
| `ft_isprint` | Checks for a printable character |
| `ft_tolower` | Converts a character to lowercase |
| `ft_toupper` | Converts a character to uppercase |
| `ft_strlen` | Returns the length of a string |
| `ft_memset` | Fills memory with a constant byte |
| `ft_bzero` | Zeroes out a byte range of memory |
| `ft_memcpy` | Copies memory area |
| `ft_memmove` | Copies memory area (handles overlap) |
| `ft_strlcpy` | Copies a string with size limiting |
| `ft_strlcat` | Concatenates strings with size limiting |
| `ft_memchr` | Scans memory for a byte |
| `ft_memcmp` | Compares memory areas |
| `ft_strnstr` | Locates a substring within a bounded length |
| `ft_strncmp` | Compares two strings up to n bytes |
| `ft_atoi` | Converts a string to an integer |
| `ft_calloc` | Allocates and zero-initializes memory |
| `ft_strdup` | Duplicates a string |

### Additional (custom) functions
| Function | Description |
|---|---|
| `ft_substr` | Extracts a substring from a string |
| `ft_strjoin` | Concatenates two strings into a new one |
| `ft_strtrim` | Trims leading/trailing characters from a string |
| `ft_split` | Splits a string into an array of substrings by delimiter |
| `ft_itoa` | Converts an integer to a string |
| `ft_strmapi` | Applies a function to each character of a string, returning a new string |
| `ft_striteri` | Applies a function to each character of a string in place |
| `ft_putchar_fd` | Outputs a character to a given file descriptor |
| `ft_putstr_fd` | Outputs a string to a given file descriptor |
| `ft_putendl_fd` | Outputs a string followed by a newline to a given file descriptor |
| `ft_putnbr_fd` | Outputs an integer to a given file descriptor |

## Resources

While building and debugging this library, the following resources were especially helpful:

- **[Bash Reference Manual / GNU User Manuals](https://www.gnu.org/software/bash/manual/)** — used for understanding shell behavior, exit codes, and Makefile-related shell interactions.
- **[Stack Overflow](https://stackoverflow.com/)** — used to troubleshoot edge cases, undefined behavior, memory management issues (malloc/free), and compare implementation approaches for functions like `ft_split` and `ft_strtrim`.

## Author

[bckblt](https://github.com/bckblt) — 42 School
