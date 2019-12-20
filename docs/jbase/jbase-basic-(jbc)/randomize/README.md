# RANDOMIZE

**Created At:** 12/11/2018 5:48:02 PM  
**Updated At:** 12/11/2018 6:20:54 PM  

**Tags:**
<badge text='rnd' vertical='middle' />
<badge text='randomize' vertical='middle' />

DESCRIPTION

Use the RANDOMIZE statement with an expression to make the RND function generate the same sequence of random numbers each time the program is run.

expression must be a positive integer or zero.

If no expression is supplied, or if *expression*evaluates to a null value, the internal time of day is used (the null value is ignored). In these cases, the sequence is different each time the program is run.

```
RANDOMIZE [(expression)]
```



An example of use would be as:

```
RANDOMIZE (0)
FOR N=1 TO 10
    PRINT RND(4):' ':
NEXT N
PRINT
*
RANDOMIZE (0)
FOR N=1 TO 10
    PRINT RND(4):' ':
NEXT N
PRINT
*
RANDOMIZE (3)
FOR N=1 TO 10
    PRINT RND(4):' ':
NEXT N
PRINT

This is the program output:
0 2 1 2 0 2 1 2 1 1
0 2 1 2 0 2 1 2 1 1
2 0 1 1 2 1 0 1 2 3
```