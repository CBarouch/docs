# SetPropertiesRequest (jbasejdbc   API)

**Created At:** 9/25/2017 11:03:57 AM  
**Updated At:** 2/15/2018 8:02:54 AM  
**Original Doc:** [com_jbase_jdbc_protocol_SetPropertiesRequest](https://docs.jbase.com/39240-protocol/com_jbase_jdbc_protocol_SetPropertiesRequest)  
**Original ID:** 277997  
**Internal:** Yes  

<!--<br>    try {<br>        if (location.href.indexOf('is-external=true') == -1) {<br>            parent.document.title="SetPropertiesRequest (jbasejdbc   API)";<br>        }<br>    }<br>    catch(err) {<br>    }<br>//--><br>var methods = {"i0":10,"i1":10,"i2":10};<br>var tabs = {65535:["t0","All Methods"],2:["t2","Instance Methods"],8:["t4","Concrete Methods"]};<br>var altColor = "altColor";<br>var rowColor = "rowColor";<br>var tableTab = "tableTab";<br>var activeTableTab = "activeTableTab";
JavaScript is disabled on your browser.

Skip navigation links

- [Overview](../../../../overview-summary.html)
- [Package](./../com.jbase.jdbc.protocol-%28jbasejdbc---api%29)
- Class
- [Use](./../class-use/uses-of-class-com.jbase.jdbc.protocol.setpropertiesrequest-%28jbasejdbc---api%29)
- [Tree](./../com.jbase.jdbc.protocol-class-hierarchy-%28jbasejdbc---api%29)
- [Deprecated](../../../../deprecated-list.html)
- [Help](../../../../help-doc.html)


jbasejdbc <br>

- [Prev Class](./../row-%28jbasejdbc---api%29 "class in com.jbase.jdbc.protocol")
- [Next Class](./../setpropertiesresponse-%28jbasejdbc---api%29 "class in com.jbase.jdbc.protocol")


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

## Class SetPropertiesRequest

- [java.lang.Object](http://java.sun.com/j2se/1.5.0/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang")
- - [com.jbase.jdbc.protocol.SQLStartRequest](./../sqlstartrequest-%28jbasejdbc---api%29 "class in com.jbase.jdbc.protocol")
    - - [com.jbase.jdbc.protocol.SQLRequest](./../sqlrequest-%28jbasejdbc---api%29 "class in com.jbase.jdbc.protocol")
        - - com.jbase.jdbc.protocol.SetPropertiesRequest


- All Implemented Interfaces:[JBaseSerializable](./../../io/jbaseserializable-%28jbasejdbc-api%29 "interface in com.jbase.jdbc.io")
* * *


```
public class SetPropertiesRequest
extends SQLRequest
```

- - ### Nested Class Summary

        - ### Nested classes/interfaces inherited from interface com.jbase.jdbc.io.[JBaseSerializable](./../../io/jbaseserializable-%28jbasejdbc-api%29 "interface in com.jbase.jdbc.io")
`JBaseSerializable.TYPE`


    - ### Field Summary

        - ### Fields inherited from class com.jbase.jdbc.protocol.[SQLRequest](./../sqlrequest-%28jbasejdbc---api%29 "class in com.jbase.jdbc.protocol")
`log, statementId`


    - ### Constructor Summary


Constructors | Constructor and Description |
| --- |
| `SetPropertiesRequest(Properties props)`  |


    - ### Method Summary


All Methods [Instance Methods](javascript:show%282%29;) [Concrete Methods](javascript:show%288%29;) | Modifier and Type | Method and Description |
| --- | --- |
| `int` | `getType()`<br>This method must be overridden by classes inheriting from SQLStartRequest.<br> |
| `void` | `readObject(JBaseObjectReader reader,<br>          int version)`  |
| `void` | `writeObject(JBaseObjectWriter writer,<br>           int version)`<br>As a bare minimum each JDBC request contains statement ID.<br> |


        - ### Methods inherited from class com.jbase.jdbc.protocol.[SQLStartRequest](./../sqlstartrequest-%28jbasejdbc---api%29 "class in com.jbase.jdbc.protocol")
`getVersion`


        - ### Methods inherited from class java.lang.[Object](http://java.sun.com/j2se/1.5.0/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang")
`clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

- - ### Constructor Detail

        - #### SetPropertiesRequest

```
public SetPropertiesRequest(Properties props)
```


    - ### Method Detail

        - #### getType

```
public int getType()
```

Description copied from class: `SQLStartRequest`

This method must be overridden by classes inheriting from SQLStartRequest.
Specified by:`getType` in interface `JBaseSerializable`Overrides:`getType` in class `SQLStartRequest`Returns:type id of the objects, used during the serialization


        - #### writeObject

```
public void writeObject(JBaseObjectWriter writer,
                        int version)
                 throws IOException
```

Description copied from class: `SQLRequest`

As a bare minimum each JDBC request contains statement ID.<br> Derived classes which override this method should take care of serializing / deserializing<br> of the statement ID on their own.
Specified by:`writeObject` in interface `JBaseSerializable`Overrides:`writeObject` in class `SQLRequest`Throws:`IOException`


        - #### readObject

```
public void readObject(JBaseObjectReader reader,
                       int version)
                throws IOException,
                       ClassNotFoundException
```
Specified by:`readObject` in interface `JBaseSerializable`Overrides:`readObject` in class `SQLRequest`Throws:`IOException``ClassNotFoundException`

Skip navigation links

- [Overview](../../../../overview-summary.html)
- [Package](./../com.jbase.jdbc.protocol-%28jbasejdbc---api%29)
- Class
- [Use](./../class-use/uses-of-class-com.jbase.jdbc.protocol.setpropertiesrequest-%28jbasejdbc---api%29)
- [Tree](./../com.jbase.jdbc.protocol-class-hierarchy-%28jbasejdbc---api%29)
- [Deprecated](../../../../deprecated-list.html)
- [Help](../../../../help-doc.html)


jbasejdbc <br>

- [Prev Class](./../row-%28jbasejdbc---api%29 "class in com.jbase.jdbc.protocol")
- [Next Class](./../setpropertiesresponse-%28jbasejdbc---api%29 "class in com.jbase.jdbc.protocol")


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
