# GETLIST

**Created At:** 9/6/2017 12:46:50 PM  
**Updated At:** 1/5/2018 1:49:53 PM  


# Description

**GETLIST**allows the program to retrieve a previously stored list (perhaps created with the **SAVE-LIST** command), into a variable. It takes the general form:

```
GETLIST expression TO variable1 {SETTING variable2} THEN|ELSE statements
```

Where:

- variable1 is the variable into which the list will be read.
- expression should evaluate to the name of a previously stored list to retrieve, or null. If expression evaluates to null, the current default external select list (generated by a previous [SELECT](278801-select) command for example) will be retrieved.
- If specified, variable2 will be set to the number of elements in the list.
- If the statement succeeds in retrieving the list, then the statements associated with any THEN clause will be executed. If the statement fails to find the list, then the statements associated with any ELSE clause will be executed.


The **GETLIST** statement is identical in function to the [READLIST](278658-readlist) statement.

An example of use is as:

```
GETLIST "MyList" TO MyList ELSE STOP
* Loop until there are no more elements
LOOP WHILE READNEXT Key FROM MyList DO
......
REPEAT
```



See also: [DELETELIST](268475-deletelist), [WRITELIST](279569-writelist)

Go back to[jBASE BASIC](263498-jbase-basic).

