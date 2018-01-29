# [NormEZ]

Coding-style checker for Epitech students. This program analyzes your C source files for [Epitech coding-style] violations.

*FR:* Moulinette de norme pour les étudiants d'Epitech. Cette norminette cherche des erreurs de [norme Epitech][Epitech coding-style] dans vos fichers de code source C.

<img alt="Epitech logo" src="/artwork/epitech-logo.png" width="304" height="144"/>

## Table of contents

* __[Getting started](#getting-started)__
  * [Requirements](#requirements)
  * [How to use NormEZ?](#how-to-use-normez)
* __[Features](#features)__
* __[To-do](#to-do)__
* __[Bugs](#bugs)__
  * [Known issues](#known-issues)
  * [Report a bug](#report-a-bug)
* __[Getting involved](#getting-involved)__
  * [Share](#share)
  * [Contribute](#contribute)
* __[Author](#author)__

## Getting started

### Requirements

 - [Ruby](https://www.ruby-lang.org/en/)

#### Installing Ruby on Fedora (Epitech's dump 2017)

```
sudo dnf install ruby
```

### How to use NormEZ?

 - Clone the repository:
```
git clone https://github.com/ronanboiteau/NormEZ
```
 - Copy the `NormEZ.rb` executable in your project repository.
 - Run NormEZ:
```
ruby NormEZ.rb
```
 - NormEZ will recursively search for `.c` and `.h` files to analyze in your current directory.

## Features

Here are the [Epitech coding-style] violations checked by NormEZ:
 - Lines with too many columns (> 80).
 - Forbidden files: every regular file that does not match `Makefile`, `*.c` or `*.h` (ex: `*.o`, `*.gch`, `bsq`, ...).
 - *[Not exhaustive]* Too broad filenames (ex: `string.c`, `algo.c`, `my_algorithm.c`, ...).
 - Missing or corrupted header.
 - Missing or corrupted header in `Makefile`.
 - Functions that contain more than 20 lines.
 - Several semicolon-separated assignments on the same line.
 - Forbidden keyword (`goto`).
 - *[Not exhaustive]* Forbidden function (`printf()`, `dprintf()`, `atoi()`, `memcpy()`, `scanf()`, `strlen()`, `strdup()`, ...).
 - Too many `else if` statements.
 - Trailing space(s) and/or tabulation(s) at the end of a line.
 - Space(s) in indentation.
 - Too many functions in file (> 5).
 - Functions with no parameters that don't take void as argument in their declaration.
 - Functions with too many arguments (> 4).
 - Missing space after keyword.
 - Misplaced pointer symbol(s).
 - Filenames that don't respect the [snake_case naming convention](https://en.wikipedia.org/wiki/Snake_case).
 - Macros used for constants.
 - Macros containing multiple assignments.
 - Misplaced comments.
 - Missing  space after comma.
 - Missing space around binary or ternary operator (`=`, `==`, `!=`, `<=`, `>=`, `&&`, `||`, `+=`, `-=`, `*=`, `/=`, `%=`, `&=`, `^=`, `|=`, `|`, `^`, `>>`, `<<`, `>>=`, `<<=`).
 - Extra space after unary operators (`!`, `sizeof`, `++`, `--`).
 - Condition and assignment on the same line.
 - Directory names that don't respect the [snake_case naming convention](https://en.wikipedia.org/wiki/Snake_case).

## To-do

Here are the [Epitech coding-style] violations ***NOT YET*** checked by NormEZ:
 - Wrong indentation level in `.c` and `.h` files.
 - Wrong indentation level in pre-processor directives.
 - Functions must be separated by *one and only one* empty line in `.c` files.
 - Extra space between function name and opening parenthesis.
 - Misplaced curly brackets.
 - Multiple variables declared on the same line.
 - Variable not declared at the beginning of function.
 - Missing empty line after variable declarations.
 - Extra empty lines.
 - Typedef not ending with `_t`
 - Identifiers that don't respect the [snake_case naming convention](https://en.wikipedia.org/wiki/Snake_case).
 - Macros, global constants or enums that don't respect the SNAKE_CASE convention (uppercase [snake_case](https://en.wikipedia.org/wiki/Snake_case)).
 - Nested conditonal branchings (depth > 2).
 - Function prototypes, typedefs, global variables, macros or static inline functions in `.c` source files.
 - Header files not protected against double inclusion

## Bugs

### Known issues

 - NormEZ doesn't make the difference between strings/comments & code. Examples: a commented forbidden function will be flagged, as well as a commented `;` (multiple assignments on the same line), etc.

### Report a bug

If you found a bug that isn't listed above in as a known issue, feel free to [create a GitHub issue](https://github.com/ronanboiteau/NormEZ/issues).

## Getting involved

### Share

 - Leave NormEZ [a star](https://github.com/ronanboiteau/NormEZ/stargazers)
 - Share the link to this repository with your friends at Epitech

### Contribute

You want to add awesome features to NormEZ? Here's how:
 1. [Fork](https://github.com/ronanboiteau/NormEZ/network/members) NormEZ
 2. Commit & push a new feature to the forked repository
 3. Open a [pull request](https://github.com/ronanboiteau/NormEZ/pulls) so I can merge your work in this repository :)

## Author

* **Ronan Boiteau** ([GitHub](https://github.com/ronanboiteau) / [LinkedIn](https://www.linkedin.com/in/ronanboiteau/))

<!-- Links -->
[Epitech coding-style]: /epitech_c_coding_style.pdf
[NormEZ]: https://github.com/ronanboiteau/NormEZ
