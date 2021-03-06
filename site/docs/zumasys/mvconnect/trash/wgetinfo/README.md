# WGETINFO

**Created At:** 6/27/2017 12:02:12 AM  
**Updated At:** 6/27/2017 11:07:52 PM  
**Original Doc:** [261265-wgetinfo](https://docs.zumasys.com/36617-trash/261265-wgetinfo)  
**Original ID:** 261265  
**Internal:** Yes  


The WGETINFO subroutine allows you return directly information from WWW.INFO common.

#### **COMMAND SYNTAX**

```
CALL WGETINFO(POS,VALUE)
```

#### **SYNTAX ELEMENTS**


| <!----> | <!----> |
| --- | --- |
| Parameter | Description |
| POS | [WWW.INFO](//WWW.INFO) Dynamic position you wish to get. |
| VALUE | Returned Value |


#### EXAMPLE

```
* Dynamically find all Variables passed by client
CALL WGETINFO(25,VAR.NAMES)
NUM.VARS=DCOUNT(VAR.NAMES,@AM)
FOR V=1 TO NUM.VARS
  VAR.NAME=VAR.NAMES<V>
  CALL WGETVAR(VALUE,VAR.NAME)
    PRINT VAR.NAME:"=":VALUE
NEXT V
```



#### **NOTES**

See WWW.INFO for details on the common.
