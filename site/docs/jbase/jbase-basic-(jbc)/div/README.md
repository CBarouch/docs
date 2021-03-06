# DIV

**Created At:** 8/23/2017 1:51:46 PM  
**Updated At:** 10/24/2018 11:01:00 PM  
**Original Doc:** [268483-div](https://docs.jbase.com/36868-jbase-basic/268483-div)  
**Original ID:** 268483  
**Internal:** No  

**Tags:**
<badge text='mathematical operations' vertical='middle' />

## Description

The **DIV** function is used to calculate the value of the quotient after division of the dividend by the divisor.

```
DIV(dividend, divisor)
```

The **dividend** and **divisor** expressions can evaluate to any numeric value. The only exception is that the divisor cannot be zero. If either dividend or divisor evaluates to null, it returns null.

An example is as below:

```
DIVIDEND = 400; DIVISOR = 2000
QUOTIENT = DIV(DIVIDEND, DIVISOR)
PRINT QUOTIENT
```

The above will output '0.2'.

Go back to [jBASE BASIC](./../jbase-basic-programmers-reference-guide).
