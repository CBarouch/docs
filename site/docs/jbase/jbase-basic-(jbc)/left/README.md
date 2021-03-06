# LEFT

**Created At:** 9/14/2017 1:44:43 PM  
**Updated At:** 11/27/2018 8:40:53 AM  
**Original Doc:** [276812-left](https://docs.jbase.com/36868-jbase-basic/276812-left)  
**Original ID:** 276812  
**Internal:** No  

**Tags:**
<badge text='string handling' vertical='middle' />

## Description

The **LEFT()** function extracts a sub-string of a specified length from the beginning of a string.

```
LEFT(expression, length)
```

Where:

- **expression** evaluates to the string from which the sub string is extracted.
- **length** is the number of extracted characters if length is less than 1, **LEFT()** returns null.

## Note

> The **LEFT** function is equivalent to sub-string extraction starting from the first character position, i.e. expression[1,length]

An example of use is as:

```
      STR_VAL =" Today's Brush is Tomorrows Forest.- Bemba Proverb"
      CRT LEFT(STR_VAL, 14)
      CRT DQUOTE(LEFT(STR_VAL,999))
      CRT DQUOTE(LEFT(STR_VAL,0))
```

to display:

```
Today's Brush
" Today's Brush is Tomorrows Forest.- Bemba Proverb"
""
```

to the screen.

See also: [RIGHT](./../right)

Go back to [jBASE BASIC](./../jbase-basic-programmers-reference-guide).
