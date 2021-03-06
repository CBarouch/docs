# SQLStartRequest (jbasejdbc   API)

**Created At:** 9/25/2017 11:04:55 AM  
**Updated At:** 2/15/2018 8:02:54 AM  
**Original Doc:** [com_jbase_jdbc_protocol_SQLStartRequest](https://docs.jbase.com/39240-protocol/com_jbase_jdbc_protocol_SQLStartRequest)  
**Original ID:** 278006  
**Internal:** Yes  

<!--<br>    try {<br>        if (location.href.indexOf('is-external=true') == -1) {<br>            parent.document.title="SQLStartRequest (jbasejdbc   API)";<br>        }<br>    }<br>    catch(err) {<br>    }<br>//--><br>var methods = {"i0":10,"i1":10};<br>var tabs = {65535:["t0","All Methods"],2:["t2","Instance Methods"],8:["t4","Concrete Methods"]};<br>var altColor = "altColor";<br>var rowColor = "rowColor";<br>var tableTab = "tableTab";<br>var activeTableTab = "activeTableTab";
JavaScript is disabled on your browser.

Skip navigation links

- [Overview](../../../../overview-summary.html)
- [Package](./../com.jbase.jdbc.protocol-%28jbasejdbc---api%29)
- Class
- [Use](./../class-use/uses-of-class-com.jbase.jdbc.protocol.sqlstartrequest-%28jbasejdbc-api%29)
- [Tree](./../com.jbase.jdbc.protocol-class-hierarchy-%28jbasejdbc---api%29)
- [Deprecated](../../../../deprecated-list.html)
- [Help](../../../../help-doc.html)


jbasejdbc <br>

- [Prev Class](./../sqlrsmdresponse-%28jbasejdbc---api%29 "class in com.jbase.jdbc.protocol")
- [Next Class](./../sqlupdateresponse-%28jbasejdbc---api%29 "class in com.jbase.jdbc.protocol")


- [Frames](./.)
- [No Frames](./.)


- [All Classes](../../../../allclasses-noframe.html)


<!--<br>  allClassesLink = document.getElementById("allclasses\_navbar\_top");<br>  if(window==top) {<br>    allClassesLink.style.display = "block";<br>  }<br>  else {<br>    allClassesLink.style.display = "none";<br>  }<br>  //-->

- Summary:
- Nested |
- Field |
- Constr |
- Method


- Detail:
- Field |
- Constr |
- Method

com.jbase.jdbc.protocol

## Class SQLStartRequest

- [java.lang.Object](http://java.sun.com/j2se/1.5.0/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang")
- - com.jbase.jdbc.protocol.SQLStartRequest


- All Implemented Interfaces:[JBaseSerializable](./../../io/jbaseserializable-%28jbasejdbc-api%29 "interface in com.jbase.jdbc.io")Direct Known Subclasses:[CompileRequest](./../compilerequest-%28jbasejdbc---api%29 "class in com.jbase.jdbc.protocol"), [DatabaseMetaDataRequest](./../databasemetadatarequest-%28jbasejdbc---api%29 "class in com.jbase.jdbc.protocol"), [LoadSubroutineRequest](./../loadsubroutinerequest-%28jbasejdbc---api%29 "class in com.jbase.jdbc.protocol"), [SQLRequest](./../sqlrequest-%28jbasejdbc---api%29 "class in com.jbase.jdbc.protocol")
* * *


```
public abstract class SQLStartRequest
extends Object
implements JBaseSerializable
```

Base class of all JDBC driver's requests.<br><br> Derived classes should override method getType, and both methods {write|read}Object<br> if they want to serialize / deserialize attributes other then statementId.
Author:Peter Kuchta

- - ### Nested Class Summary

        - ### Nested classes/interfaces inherited from interface com.jbase.jdbc.io.[JBaseSerializable](./../../io/jbaseserializable-%28jbasejdbc-api%29 "interface in com.jbase.jdbc.io")
`JBaseSerializable.TYPE`


    - ### Field Summary


Fields | Modifier and Type | Field and Description |
| --- | --- |
| `protected static Logger` | `log`  |


    - ### Constructor Summary


Constructors | Constructor and Description |
| --- |
| `SQLStartRequest()`  |


    - ### Method Summary


All Methods [Instance Methods](javascript:show%282%29;) [Concrete Methods](javascript:show%288%29;) | Modifier and Type | Method and Description |
| --- | --- |
| `int` | `getType()`<br>This method must be overridden by classes inheriting from SQLStartRequest.<br> |
| `int` | `getVersion()`  |


        - ### Methods inherited from class java.lang.[Object](http://java.sun.com/j2se/1.5.0/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang")
`clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`


        - ### Methods inherited from interface com.jbase.jdbc.io.[JBaseSerializable](./../../io/jbaseserializable-%28jbasejdbc-api%29 "interface in com.jbase.jdbc.io")
`readObject, writeObject`

- - ### Field Detail

        - #### log

```
protected static final Logger log
```


    - ### Constructor Detail

        - #### SQLStartRequest

```
public SQLStartRequest()
```


    - ### Method Detail

        - #### getType

```
public int getType()
```

This method must be overridden by classes inheriting from SQLStartRequest.
Specified by:`getType` in interface `JBaseSerializable`Returns:type id of the objects, used during the serialization


        - #### getVersion

```
public int getVersion()
```
Specified by:`getVersion` in interface `JBaseSerializable`

Skip navigation links

- [Overview](../../../../overview-summary.html)
- [Package](./../com.jbase.jdbc.protocol-%28jbasejdbc---api%29)
- Class
- [Use](./../class-use/uses-of-class-com.jbase.jdbc.protocol.sqlstartrequest-%28jbasejdbc-api%29)
- [Tree](./../com.jbase.jdbc.protocol-class-hierarchy-%28jbasejdbc---api%29)
- [Deprecated](../../../../deprecated-list.html)
- [Help](../../../../help-doc.html)


jbasejdbc <br>

- [Prev Class](./../sqlrsmdresponse-%28jbasejdbc---api%29 "class in com.jbase.jdbc.protocol")
- [Next Class](./../sqlupdateresponse-%28jbasejdbc---api%29 "class in com.jbase.jdbc.protocol")


- [Frames](./.)
- [No Frames](./.)


- [All Classes](../../../../allclasses-noframe.html)


<!--<br>  allClassesLink = document.getElementById("allclasses\_navbar\_bottom");<br>  if(window==top) {<br>    allClassesLink.style.display = "block";<br>  }<br>  else {<br>    allClassesLink.style.display = "none";<br>  }<br>  //-->

- Summary:
- Nested |
- Field |
- Constr |
- Method


- Detail:
- Field |
- Constr |
- Method

*Copyright © 2017 jBASE, Inc.. All Rights Reserved.*
