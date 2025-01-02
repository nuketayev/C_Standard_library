# C Standard Library Implementation

This project is a custom implementation of the C Standard Library functions. The goal of this project is to provide a comprehensive set of functions that mimic the behavior of the standard C library functions, as well as additional utility functions.

## Functions Implemented

The library includes the following functions:

### Standard Library Functions

- `ft_atoi`
- `ft_bzero`
- `ft_calloc`
- `ft_isalnum`
- `ft_isalpha`
- `ft_isascii`
- `ft_isdigit`
- `ft_isprint`
- `ft_itoa`
- `ft_memchr`
- `ft_memcmp`
- `ft_memcpy`
- `ft_memmove`
- `ft_memset`
- `ft_putchar_fd`
- `ft_putendl_fd`
- `ft_putnbr_fd`
- `ft_putstr_fd`
- `ft_split`
- `ft_strchr`
- `ft_strdup`
- `ft_striteri`
- `ft_strjoin`
- `ft_strlcat`
- `ft_strlcpy`
- `ft_strlen`
- `ft_strmapi`
- `ft_strncmp`
- `ft_strnstr`
- `ft_strrchr`
- `ft_strtrim`
- `ft_substr`
- `ft_tolower`
- `ft_toupper`

### Additional Functions

- `ft_lstadd_back`
- `ft_lstadd_front`
- `ft_lstclear`
- `ft_lstdelone`
- `ft_lstiter`
- `ft_lstlast`
- `ft_lstmap`
- `ft_lstnew`
- `ft_lstsize`

## Compilation

To compile the library, use the provided `Makefile`. The `Makefile` defines the following targets:

- `all`: Compiles the library.
- `clean`: Removes object files.
- `fclean`: Removes object files and the library.
- `re`: Recompiles the library.
- `bonus`: Compiles the library with bonus functions.

To compile the library, run the following command:

```sh
make
```

To compile the library with bonus functions, run the following command:

```sh
make bonus
```

## Usage Examples

Here are some examples of how to use the functions provided by the library:

### Example 1: Using `ft_atoi`

```c
#include "libft.h"
#include <stdio.h>

int main() {
    char *str = "42";
    int num = ft_atoi(str);
    printf("The number is: %d\n", num);
    return 0;
}
```

### Example 2: Using `ft_split`

```c
#include "libft.h"
#include <stdio.h>

int main() {
    char *str = "Hello World";
    char **words = ft_split(str, ' ');
    for (int i = 0; words[i] != NULL; i++) {
        printf("Word %d: %s\n", i, words[i]);
    }
    return 0;
}
```

### Example 3: Using `ft_strjoin`

```c
#include "libft.h"
#include <stdio.h>

int main() {
    char *s1 = "Hello";
    char *s2 = "World";
    char *joined = ft_strjoin(s1, s2);
    printf("Joined string: %s\n", joined);
    return 0;
}
```
