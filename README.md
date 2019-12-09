# Objective

The objective of this lab is to implement the rest of the [static type checking](https://en.wikipedia.org/wiki/Type_system#Static_type_checking) for the subset of Java: 

  * infix expressions
  * unary expressions
  * `new` expressions
  * method invocation
  * if-statements
  * while-statements
  * do-while-statements
  * return statements

The other objective is to test the fitness of the tests with mutation analysis. 

The program will take no arguments as input and can only be invoked through the tests. The program should only apply to the limited subset of Java defined in [lab3-type-checking-p1](https://github.com/byu-cs329/lab3-type-checking-p1). If an input file is outside the subset, then it should throw an appropriate run-time exception.

# Reading

Review carefully the [type checking](https://bitbucket.org/byucs329/byu-cs-329-lecture-notes/src/master/type-checking.md) lecture with its companion slides [09-type-checking.ppt](https://bitbucket.org/byucs329/byu-cs-329-lecture-notes/src/master/compilers/09-type-checking.ppt).

# Lab Requirements

## Type Proofs

Implement the dynamic test generation for the static type proof for the following language features. 

  * `InfixExpression`
  * `PrefixExpression`
  * `ParenthesizedExpression`
  * `ClassInstanceCreation`
  * `MethodInvocation`
  * `IfStatement`
  * `WhileStatement`
  * `DoStatement`
  * `ReturnStatement`

## Testing your test code?

Write any tests deemed sufficient to cover the implementation of the type-checker to create an appropriate regression test suite. Analyze the fitness of the regression tests using [PIT](http://pitest.org) for mutations analysis with the `NEW_DEFUALT` group and `RETURN_VALS` as mutators. Add tests to kill all mutants or argue why a mutant cannot be killed. Clearly indicate where the explanations are located in the pull request.

# What to turn in?

Create a pull request when the lab is done. Submit to Canvas the URL of the repository.

# Rubric

| Item | Point Value |
| ------- | ----------- |
| `InfixExpressions` | 20 |
| `PrefixExpressions` | 5 |
| `ParenthesizedExpressions` | 5 |
| `MethodInvocation` | 20 |
| `IfStatement` | 15 |
| `WhileStatement` | 15 |
| `DoStatement` | 15 | 
| `ReturnStatement` | 5 |
| Sufficient tests to kill mutants with `NEW_DEFAULT` and `RETURN_VALS` or justification | 70 | 
| Style, documentation, naming conventions, test organization, readability, etc. | 30 | 