# PROCWRITE

**Created At:** 10/25/2017 2:54:59 PM  
**Updated At:** 4/3/2018 8:58:50 PM  


# Description 

**PROCWRITE**is used to pass data back to the primary input buffer of a calling jCL program. It takes the general form:

```
PROCWRITE expression
```

where expression may evaluate to any valid data type.

An example of use may be as:

```
PROCWRITE "Success":CHAR (254):"0"
```

See also: [PROCREAD](277635-procread)

Go back to [jBASE BASIC](263498-jbase-basic).
