# JBASE_ERRMSG_NON_NUMERIC

**Created At:** 11/3/2017 5:03:03 PM  
**Updated At:** 10/26/2018 1:10:39 PM  
**Original Doc:** [jbase_errmsg_non_numeric](https://docs.jbase.com/41717-environment-variables/jbase_errmsg_non_numeric)  
**Original ID:** 284180  
**Internal:** No  


## **Description**

Defines behavior when a BASIC program encounters a numeric operation being attempted on a non-numeric value. The default behavior is to raise an error and drop into the debugger.

## 


## Values

- 1 - Don't display an error message
- 2 - Don't enter the debugger
- 16 - Caller to place "0" in the target variable after operation
- 2 - Caller to place "" (null) in the target variable after operation
- 64 - Caller to leave target variable alone after operation
- 128 - Caller to place source variable in the target variable after operation


## 


## **Default**

0 - Raise an error and drop into the debugger

## 


## **Setting**

The value stored in a bit mask so different behaviors can be combined by adding them together.

For example, to suppress the error message and avoid going into the debugger, set the variable to 3.

As per normal environment variables, it can be set at any time or in a BASIC program with the jBC [PUTENV](./../../jbase-basic-%28jbc%29/putenv)function.

### Unix

```
export JBASE_ERRMSG_NON_NUMERIC=3
```

### Windows

```
set JBASE_ERRMSG_NON_NUMERIC=3
```



Back to [Error Handling](./../../jbase-basic-%28jbc%29/jbc-error-handling)
