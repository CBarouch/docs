# SIN

**Created At:** 9/28/2017 9:25:58 AM  
**Updated At:** 1/5/2018 6:17:24 PM  
**Original Doc:** [278808-sin](https://docs.jbase.com/36868-jbase-basic/278808-sin)  
**Original ID:** 278808  
**Internal:** No  

## Description

The **SIN** function returns the mathematical sine value of a numeric expression. The function has the general form:

```
SIN(expression)
```

Where:

**expression** should evaluate to a numeric value and is interpreted as a number of degrees between 0 and 360.

The function will calculate the sine of the angle specified by **expression** as accurately as the host system will allow. It will then truncate the value according to the [PRECISION](./../precision) of the program.

Examples of use would be:

```
CRT @ (-1):
FOR I = 0 TO 79
    CRT @ (I,12+INT(SIN (360/80*(I+1))*10)):"*":
NEXT I
```

or

```
PRECISION 2
CRT SIN(39)
```

to display the sine of 39 to two decimal places.

Go back to [jBASE BASIC](./../jbase-basic-programmers-reference-guide).
