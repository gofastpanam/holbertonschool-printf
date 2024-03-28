# C - printf

## Description of the project
Create our own printf function. printf is the C language function to do formatted printing.

## Evironment
- Operating system : Ubuntu 20.04 LTS
- Compiler : gcc 9.3.0
- GCC options : Wall -Werror -Wextra -pedantic -std=gnu89

## Project specifitacation
- All files end with a new line
- No allowed to use global variable
- No more than 5 functions per file
- There is one project repository per group

## Examples
_printf functions examples:

- _printf("Character:[%c]\n", 'H');
  + Output: char: [H]
- _printf("String:[%s]\n", "I am a string !");
  + Output: string: [I am a string !]
- _printf("Percent: [%%]\n");
  + Output: Percent: [%%]
- _printf("decimal: [%d]\n", 10000);
  + Output: decimal: [10000]
- _printf("decimal: [%i]\n", 10000);
  + Output: decimal: [10000]

## Man page
```
NAME
	_printf - Print formatted output to stdout

SYNOPSIS
	#include <stdio.h>
	int _printf(const char *format, ...);

DESCRIPTION
	The _printf function formats and prints data to the standard output stream (stdout). It accepts a format string format followed by optional arguments. Within the format string, conversion specifiers begin with the '%' character, followed by optional flags, field width, precision, and length modifiers, then a conversion specifier character.

	Conversion Specifiers:
	%c: character
	%s: string
	%d, %i: signed decimal integer
	%u: unsigned decimal integer
	%x, %X: unsigned hexadecimal integer (lowercase/uppercase)
	%f, %lf: floating-point number (single/double precision)
	%p: pointer address
	%%: percentage sign

Flags:
	+: Forces to preceed the result with a plus or minus sign (+ or -)
	-: Left-justify within the given field width
	0: Pads with zeros instead of spaces
	(space): If no sign is going to be written, a blank space is inserted before the value.

Field Width:
	An optional decimal digit string that specifies the minimum field width.

Precision:
	An optional precision that specifies the minimum number of digits to be printed for d, i, o, u, x, X, and f conversions.

Length Modifier:
	h: Indicates that the d, i, o, u, x, X conversion specifier applies to a short int or unsigned short int.
	l: Indicates that the d, i, o, u, x, X conversion specifier applies to a long int or unsigned long int.
	ll: Indicates that the d, i, o, u, x, X conversion specifier applies to a long long int or unsigned long long int.
	L: Indicates that the f conversion specifier applies to a long double.

RETURN VALUE
	Upon successful completion, _printf returns the number of characters printed (excluding the null byte used to end output to strings).

EXAMPLES
	#include <stdio.h>

	int main()
    {
		int num = 42;
		char *str = "Hello, world!";
		_printf("The number is: %d\n", num);
		_printf("The string is: %s\n", str);
		return 0;
	}

DATE
	March 29, 2024

```

## Flowchart
![Flowchart](https://github.com/gofastpanam/holbertonschool-printf/blob/main/printf_flowchart.png)

Created by [Benjamin Jacob](https://github.com/gofastpanam/) & [Anthony Cointre](https://github.com/AnthonyCointre/).
