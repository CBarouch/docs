# LENS

**Created At:** 9/14/2017 2:19:44 PM  
**Updated At:** 11/27/2018 10:12:28 AM  
**Original Doc:** [276857-lens](https://docs.jbase.com/36868-jbase-basic/276857-lens)  
**Original ID:** 276857  
**Internal:** No  

**Tags:**
<badge text='dynamic arrays' vertical='middle' />

## Description

This function returns a dynamic array of the number of bytes in each element of the dynamic.array. It takes the general form:

```
LENS(dynamic.array)
```

The characters in each element of **dynamic.array** are counted, with the counts returned.

## Note

> Blank spaces (leading or trailing) are included in the calculation.
>
> If dynamic.array evaluates to a null string, it returns zero (0). If any element of dynamic.array is null, returns zero (0) for that element.

When used in International Mode, the function will return the number of characters in the specified expression rather than the number of bytes. If the expression consists entirely of UTF-8 characters in the ASCII range 0 – 127 then the character length of the expression will equate to the byte length. However, when the expression contains characters outside the ASCII range 0 – 127 then byte length and character length will differ. If the byte is specifically required then the [BYTELEN](./../bytelen) function should be used instead.

It is not recommended to use programs to manipulate byte counts in International Mode.

Go back to [jBASE BASIC](./../jbase-basic-programmers-reference-guide).
