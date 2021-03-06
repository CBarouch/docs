# INS

**Created At:** 9/8/2017 2:54:29 PM  
**Updated At:** 10/30/2018 9:46:06 AM  
**Original Doc:** [276289-ins](https://docs.jbase.com/36868-jbase-basic/276289-ins)  
**Original ID:** 276289  
**Internal:** No  

**Tags:**
<badge text='dynamic array' vertical='middle' />

## Description

The **INS** statement allows the insertion of elements into a dynamic array.

```
INS expression BEFORE Var<expression1{, expression2{, expression3}}>
```

Where:

- **expression** evaluates to the element to be inserted in the dynamic array.
- **expression1** **expression2** and **expression3** should all evaluate to numeric values and specify the Field, Value and Sub-Value before which the new element is to be inserted.

## Note

> Specifying a negative value to any of the expressions 1 through 3 will cause the element to append as the last Field, Value or Sub-Value rather than at a specific position. Only one expression may be negative otherwise only the first negative value is used correctly while the others are treated as the value 1.
>
> The statement will insert NULL Fields, Values or Sub-Values  accordingly if any of the specified insertion points exceeds the number currently existing.

An example of use is as:

```
ARR_VAL =" "
FOR I = 1 TO 5
    INS I BEFORE VAL<1>
NEXT I
```

or

```
ARR_VAL2 =" "
FOR I = 2 TO 8
    INS I*7 BEFORE ARR_VAL2<7,I>
NEXT I
```

to populate the respective arrays with values.

Go back to [jBASE BASIC](./../jbase-basic-programmers-reference-guide).
