# WGETBODY

**Created At:** 6/27/2017 12:00:23 AM  
**Updated At:** 6/27/2017 11:07:14 PM  
**Original Doc:** [261264-wgetbody](https://docs.zumasys.com/36617-trash/261264-wgetbody)  
**Original ID:** 261264  
**Internal:** Yes  


The WGETBODY gets the raw body sent in the web request.  Only certain content types pass the raw body.  See the config file to determine which ones.

### **COMMAND SYNTAX**

```
CALL WGETBODY(BODY)
```

### **SYNTAX ELEMENTS**


| <!----> | <!----> |
| --- | --- |
| Parameter | Description |
| BODY | Returned body |


The WGETBODY subroutine only returns a string.  That string is the raw body.

### EXAMPLE

```
CALL WGETBODY(BODY)
* NOW PARSE BODY JSON INTO A OBJECT
CALL WOBJ(BODYOBJ,"FROMSTRING","",BODY,"",RERR)
```
