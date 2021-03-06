# DELETE

**Created At:** 9/6/2017 7:01:24 AM  
**Updated At:** 10/30/2018 1:23:48 PM  
**Original Doc:** [276025-delete](https://docs.jbase.com/36868-jbase-basic/276025-delete)  
**Original ID:** 276025  
**Internal:** No  

**Tags:**
<badge text='records' vertical='middle' />
<badge text='file operations' vertical='middle' />

## Description

This statement is used to delete a record from a jBASE file. It takes the general form:

```
DELETE {variable,} expression {SETTING setvar} {ON ERROR statements}
```

Where:

- If specified, **variable** should have been the subject of a previous [OPEN](./../open) statement. If variable is omitted then it assumes the default file variable.
- The **expression** should evaluate to the name of a record stored in the open file.
- If the **SETTING** clause is specified and the delete fails, it sets **setvar** to one of [these file error values](./../incremental-file-errors).

## Note

> The statement will have no effect if the record name does not exist within the file. If the program against the file record was holding a lock, it will release the lock.

An example of use is as:

```
     OPEN "test_rec" TO file_variable ELSE ABORT 201, "test_rec"
     DELETE file_variable , "001"
```

to delete the record "001" from the file test\_rec .

Go back to [jBASE BASIC](./../jbase-basic-programmers-reference-guide).
