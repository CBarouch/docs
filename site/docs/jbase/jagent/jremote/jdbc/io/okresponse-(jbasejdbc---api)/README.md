# OKResponse (jbasejdbc   API)

**Created At:** 9/25/2017 10:53:45 AM  
**Updated At:** 2/15/2018 8:02:43 AM  
**Original Doc:** [com_jbase_jdbc_io_OKResponse](https://docs.jbase.com/39232-io/com_jbase_jdbc_io_OKResponse)  
**Original ID:** 277908  
**Internal:** Yes  

<!--<br>    try {<br>        if (location.href.indexOf('is-external=true') == -1) {<br>            parent.document.title="OKResponse (jbasejdbc   API)";<br>        }<br>    }<br>    catch(err) {<br>    }<br>//--><br>var methods = {"i0":10,"i1":10,"i2":10,"i3":10};<br>var tabs = {65535:["t0","All Methods"],2:["t2","Instance Methods"],8:["t4","Concrete Methods"]};<br>var altColor = "altColor";<br>var rowColor = "rowColor";<br>var tableTab = "tableTab";<br>var activeTableTab = "activeTableTab";
JavaScript is disabled on your browser.

Skip navigation links

- [Overview](../../../../overview-summary.html)
- [Package](./../com.jbase.jdbc.io-%28jbasejdbc---api%29)
- Class
- [Use](./../class-use/uses-of-class-com.jbase.jdbc.io.okresponse-%28jbasejdbc---api%29)
- [Tree](./../com.jbase.jdbc.io-class-hierarchy-%28jbasejdbc---api%29)
- [Deprecated](../../../../deprecated-list.html)
- [Help](../../../../help-doc.html)


jbasejdbc <br>

- [Prev Class](./../objectfactory-%28jbasejdbc-api%29 "class in com.jbase.jdbc.io")
- [Next Class](./../prefixbytebuffer-%28jbasejdbc-api%29 "class in com.jbase.jdbc.io")


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

com.jbase.jdbc.io

## Class OKResponse

- [java.lang.Object](http://java.sun.com/j2se/1.5.0/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang")
- - [com.jbase.jdbc.io.Response](./../response-%28jbasejdbc-api%29 "class in com.jbase.jdbc.io")
    - - com.jbase.jdbc.io.OKResponse


- All Implemented Interfaces:[JBaseSerializable](./../jbaseserializable-%28jbasejdbc-api%29 "interface in com.jbase.jdbc.io")
* * *


```
public class OKResponse
extends Response
```

- - ### Nested Class Summary

        - ### Nested classes/interfaces inherited from interface com.jbase.jdbc.io.[JBaseSerializable](./../jbaseserializable-%28jbasejdbc-api%29 "interface in com.jbase.jdbc.io")
`JBaseSerializable.TYPE`


    - ### Constructor Summary


Constructors | Constructor and Description |
| --- |
| `OKResponse()`  |


    - ### Method Summary


All Methods [Instance Methods](javascript:show%282%29;) [Concrete Methods](javascript:show%288%29;) | Modifier and Type | Method and Description |
| --- | --- |
| `int` | `getType()`  |
| `int` | `getVersion()`  |
| `void` | `readObject(JBaseObjectReader reader,<br>          int version)`  |
| `void` | `writeObject(JBaseObjectWriter writer,<br>           int version)`  |


        - ### Methods inherited from class java.lang.[Object](http://java.sun.com/j2se/1.5.0/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang")
`clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

- - ### Constructor Detail

        - #### OKResponse

```
public OKResponse()
```


    - ### Method Detail

        - #### writeObject

```
public void writeObject(JBaseObjectWriter writer,
                        int version)
                 throws IOException
```
Throws:`IOException`


        - #### readObject

```
public void readObject(JBaseObjectReader reader,
                       int version)
                throws IOException,
                       ClassNotFoundException
```
Throws:`IOException``ClassNotFoundException`


        - #### getType

```
public int getType()
```
Returns:type id of the objects, used during the serialization


        - #### getVersion

```
public int getVersion()
```

Skip navigation links

- [Overview](../../../../overview-summary.html)
- [Package](./../com.jbase.jdbc.io-%28jbasejdbc---api%29)
- Class
- [Use](./../class-use/uses-of-class-com.jbase.jdbc.io.okresponse-%28jbasejdbc---api%29)
- [Tree](./../com.jbase.jdbc.io-class-hierarchy-%28jbasejdbc---api%29)
- [Deprecated](../../../../deprecated-list.html)
- [Help](../../../../help-doc.html)


jbasejdbc <br>

- [Prev Class](./../objectfactory-%28jbasejdbc-api%29 "class in com.jbase.jdbc.io")
- [Next Class](./../prefixbytebuffer-%28jbasejdbc-api%29 "class in com.jbase.jdbc.io")


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
