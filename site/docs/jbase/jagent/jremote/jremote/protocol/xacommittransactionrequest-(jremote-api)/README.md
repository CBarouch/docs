# XACommitTransactionRequest (jremote API)

**Created At:** 9/25/2017 12:22:56 PM  
**Updated At:** 4/4/2018 9:32:39 PM  
**Original Doc:** [com_jbase_jremote_protocol_xacommittransactionrequest](https://docs.jbase.com/39270-protocol/com_jbase_jremote_protocol_xacommittransactionrequest)  
**Original ID:** 278422  
**Internal:** No  

<!--<br>    try {<br>        if (location.href.indexOf('is-external=true') == -1) {<br>            parent.document.title="XACommitTransactionRequest (jremote   API)";<br>        }<br>    }<br>    catch(err) {<br>    }<br>//--><br>var methods = {"i0":10,"i1":10};<br>var tabs = {65535:["t0","All Methods"],2:["t2","Instance Methods"],8:["t4","Concrete Methods"]};<br>var altColor = "altColor";<br>var rowColor = "rowColor";<br>var tableTab = "tableTab";<br>var activeTableTab = "activeTableTab";
JavaScript is disabled on your browser.



## Class XACommitTransactionRequest

All Implemented Interfaces:[JBaseSerializable](./../../io/jbaseserializable-%28jremote-api%29 "interface in com.jbase.jremote.io")
* * *


```
public class XACommitTransactionRequest
extends JRemoteRequest
```

Request jBASE commit an XA transaction.

### Nested Class Summary

- Nested classes/interfaces inherited from interface com.jbase.jremote.io.JBaseSerializable
    - `JBaseSerializable.TYPE`






### Constructor Summary


| Constructor and Description<br> |
| --- |
| `XACommitTransactionRequest(byte[] globalTransId, byte[] branchId, int formatId)` <br> |






### Method Summary


| Modifier and Type<br> | Method and Description<br> |
| --- | --- |
| `int`<br> | `getType()` <br> |
| `void`<br> | `writeObject(JBaseObjectWriter writer, int version)` <br> |


- Methods inherited from class com.jbase.jremote.protocol.JRemoteRequest
    - `getVersion, readObject`
- Methods inherited from class java.lang.Object
    - `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

### Constructor Detail

#### XACommitTransactionRequest

```
public XACommitTransactionRequest(byte[] globalTransId,
                                  byte[] branchId,
                                  int formatId)
```



### 


### Method Detail

#### writeObject

```
public void writeObject(JBaseObjectWriter writer,
                        int version)
                 throws IOException
```
Specified by:`writeObject` in interface `JBaseSerializable`Overrides:`writeObject` in class `JRemoteRequest`Throws:`IOException`
#### getType

```
public int getType()
```
Returns:type id of the objects, used during the serializationSee Also:[`JBaseSerializable.getType()`](./../../io/jbaseserializable-%28jremote-api%29#getType--)

Back to [jREMOTE API](com_jbase_jremote_package-summary)


