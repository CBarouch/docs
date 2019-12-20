# INSERT

**Created At:** 9/13/2017 12:40:18 PM  
**Updated At:** 10/30/2018 9:46:23 AM  

**Tags:**
<badge text='dynamic arrays' vertical='middle' />

# Description

**INSERT** is the function form of the [INS](276289-ins) statement, with preference given to the use of [INS](276289-ins). It takes the general form:

```
INSERT(expression1, expression2{, expression3 {, expression4 }}; expression5)
```

Where :

- **expression1**evaluates to a dynamic array in which to insert a new element and will normally be a variable.
- **expression2, expression3** and**expression4** should evaluate to integer values and specify the attribute, multi-value and sub-value before which the new element will be inserted.
- **expression5** evaluates to the new element to be inserted in expression1.


An example of use is as:

```
A = INSERT(B, 1, 4; "Field1Value4")
```

Note that *B*is unchanged and the modified *expression1*is assigned to the variable A.



Go back to [jBASE BASIC](263498-jbase-basic).

