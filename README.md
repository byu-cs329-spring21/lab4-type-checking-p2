# Objective

The objective of this lab is to implement the rest of the [static type checking](https://en.wikipedia.org/wiki/Type_system#Static_type_checking) for the subset of Java: 

  * infix expressions
  * unary expressions
  * method calls
  * if-statements
  * while-statements
  * do-while-statements

The other objective is to test the fitness of the tests with mutation analysis. 

The program will take no arguments as input and can only be invoked through the tests. The program should only apply to the limited subset of Java defined in [lab3-type-checking-p1](https://github.com/byu-cs329/lab3-type-checking-p1). If an input file is outside the subset, then it should throw an appropriate run-time exception.

# Reading

Review carefully the [type checking](https://bitbucket.org/byucs329/byu-cs-329-lecture-notes/src/master/type-checking.md) lecture with its companion slides [09-type-checking.ppt](https://bitbucket.org/byucs329/byu-cs-329-lecture-notes/src/master/compilers/09-type-checking.ppt).

# Lab Requirements

## Type Proofs

Implement the dynamic test generation for the static type proof for the following language features using a mock for the symbol table. 

  * Infix expressions
  * Unary expressions
  * Method calls
  * If-statements
  * While-statements
  * Do-while-statements

## Testing your test code?

Write any tests deemed sufficient to cover the implementation of the type-checker to create an appropriate regression test suite. Analyze the fitness of the regression tests using [PIT](http://pittest.org) for mutations analysis with the `NEW_DEFUALT` group and `RETURN_VALS` as mutators. Add tests to kill all mutants or argue why a mutant cannot be killed.

# What to turn in?

Create a pull request when the lab is done. Submit to Canvas the URL of the repository.

# Rubric

| Item | Point Value |
| ------- | ----------- |
| Infix Expressions | 15 |
| Unary Expressions | 15 |
| Method calls | 25 |
| If-statements | 15 |
| While-statements | 15 |
| Do-while-statements | 15 | 
| Sufficient tests to kill mutants | 70 | 
| Style, documentation, naming conventions, test organization, readability, etc. | 30 | 