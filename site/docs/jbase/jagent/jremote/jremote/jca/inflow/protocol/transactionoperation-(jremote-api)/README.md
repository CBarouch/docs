# TransactionOperation (jremote API)

**Created At:** 9/25/2017 12:05:01 PM  
**Updated At:** 4/5/2018 12:16:16 AM  
**Original Doc:** [com_jbase_jremote_jca_inflow_protocol_transactionoperation](https://docs.jbase.com/39264-protocol/com_jbase_jremote_jca_inflow_protocol_transactionoperation)  
**Original ID:** 278264  
**Internal:** No  

<!--<br>    try {<br>        if (location.href.indexOf('is-external=true') == -1) {<br>            parent.document.title="TransactionOperation (jremote   API)";<br>        }<br>    }<br>    catch(err) {<br>    }<br>//--><br>var methods = {"i0":10,"i1":10,"i2":10,"i3":10,"i4":10,"i5":10};<br>var tabs = {65535:["t0","All Methods"],2:["t2","Instance Methods"],8:["t4","Concrete Methods"]};<br>var altColor = "altColor";<br>var rowColor = "rowColor";<br>var tableTab = "tableTab";<br>var activeTableTab = "activeTableTab";
JavaScript is disabled on your browser.



## Class TransactionOperation

All Implemented Interfaces:[JBaseSerializable](./../../../../io/jbaseserializable-%28jremote-api%29 "interface in com.jbase.jremote.io")
* * *


```
public class TransactionOperation
extends Object
implements JBaseSerializable
```

### Nested Class Summary

- Nested classes/interfaces inherited from interface com.jbase.jremote.io.JBaseSerializable
    - `JBaseSerializable.TYPE`






### Constructor Summary


| Constructor and Description<br> |
| --- |
| `TransactionOperation()` <br> |
| `TransactionOperation(boolean operationSuccessful, String transId)` <br> |






### Method Summary


| Modifier and Type<br> | Method and Description<br> |
| --- | --- |
| `String`<br> | `getTransactionId()` <br> |
| `int`<br> | `getType()` <br> |
| `int`<br> | `getVersion()` <br> |
| `boolean`<br> | `isOperationSuccessful()` <br> |
| `void`<br> | `readObject(JBaseObjectReader reader, int version)` <br> |
| `void`<br> | `writeObject(JBaseObjectWriter writer, int version)` <br> |


- Methods inherited from class java.lang.Object
    - `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

### Constructor Detail



#### TransactionOperation

```
public TransactionOperation()
```





#### TransactionOperation

```
public TransactionOperation(boolean operationSuccessful,
                            String transId)
```





### 


### Method Detail



#### getType

```
public int getType()
```
Specified by:`getType` in interface `JBaseSerializable`Returns:type id of the objects, used during the serialization
#### getVersion

```
public int getVersion()
```
Specified by:`getVersion` in interface `JBaseSerializable`
#### readObject

```
public void readObject(JBaseObjectReader reader,
                       int version)
                throws IOException,
                       ClassNotFoundException
```
Specified by:`readObject` in interface `JBaseSerializable`Throws:`IOException``ClassNotFoundException`
#### writeObject

```
public void writeObject(JBaseObjectWriter writer,
                        int version)
                 throws IOException
```
Specified by:`writeObject` in interface `JBaseSerializable`Throws:`IOException`
#### getTransactionId

```
public String getTransactionId()
```

#### isOperationSuccessful

```
public boolean isOperationSuccessful()
```

Back to [jREMOTE API](com_jbase_jremote_package-summary)
