# Documentation
Documentation for the ALB Programming Language

![current version none](https://img.shields.io/badge/ALB%20current%20version-none-red.svg) ![up to date with version none](https://img.shields.io/badge/up%20to%20date%20with%20version-none-red.svg)

![docs version 0.0.2](https://img.shields.io/badge/documentation%20version-0.0.2-brightgreen.svg)

### Found a bug?

Contact us! At alblang.project@gmail.com and we will try too fix it as soon as possible.

# Basic structure of an ALB program

This is the basic structure of an ALB program. You will need this knowledge to understand and properly compile and execute ALB programs.

```
// This is a comment. Comments must be introduced by two slashes (//), and they are simply ignored by the compiler.
BEGIN
	// some code...
END
```

Every program is delimited by the `BEGIN` and `END` instructions. Any text not between these instructions will not influence the final result, nor any comment inside or outside the `BEGIN`-`END` structure.

Comments are specified by writing two slashes (`//`) at the beginning of the comment. Anything after the slashes and in the same line will be ignored. Comments are single-lined. There are not multiple-line comments in ALB.

# Table of contents
  - stdlib: ALB Standard Library.
    
    - stdout: Standard Output: usage, interaction, methods and examples.
    
    - stdin: Standard Input: usage, interaction, methods, examples and getting values from console.

  - variables: creation, interaction, information and examples.


# Version history
Key:
![released version](https://img.shields.io/badge/released-brightgreen.svg) ![in progress version](https://img.shields.io/badge/in%20progress-orange.svg) ![planned version](https://img.shields.io/badge/planned-red.svg) ![withdrawn version](https://img.shields.io/badge/withdrawn-gray.svg)
- ![0.0.1](https://img.shields.io/badge/0.0.1-brightgreen.svg): Initial release (stdout, variables, README.md, MIT License)
- ![0.0.2](https://img.shields.io/badge/0.0.2-brightgreen.svg): variables and stdin
- ![0.0.3](https://img.shields.io/badge/0.0.3-orange.svg): data types
- ![0.0.4](https://img.shields.io/badge/0.0.4-red.svg): operators
