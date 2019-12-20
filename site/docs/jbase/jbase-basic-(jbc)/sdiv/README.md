# SDIV

**Created At:** 9/28/2017 9:00:58 AM  
**Updated At:** 1/5/2018 6:14:08 PM  


# Description

The **SDIV** function performs a string division of two base 10-string numbers and rounds the result to 14 decimal places. It generally takes the form:

```
SDIV(expr1, expr2)
```

Where:

expr1 and expr2 are strings consisting of numeric characters, with either optionally including a decimal part.

Use the **SDIV** function with numbers that may exceed a valid range with standard arithmetic operators.

The [PRECISION](277629-precision) declaration has no effect on the value returned by **SDIV**.

Examples of use may be as:

```
A = 2
B = 3
CRT SDIV (A,B)
```

to display 0.66666666666666 to the screen, or

```
PRECISION 2
CRT SDIV (355,113)
```

to display 3.14159292035398.



Go back to [jBASE BASIC](263498-jbase-basic).