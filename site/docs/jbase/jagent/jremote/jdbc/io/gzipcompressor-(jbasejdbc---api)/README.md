# GZipCompressor (jbasejdbc   API)

**Created At:** 9/25/2017 10:49:22 AM  
**Updated At:** 2/15/2018 8:02:48 AM  
**Original Doc:** [com_jbase_jdbc_io_GZipCompressor](https://docs.jbase.com/39232-io/com_jbase_jdbc_io_GZipCompressor)  
**Original ID:** 277871  
**Internal:** Yes  

<!--<br>    try {<br>        if (location.href.indexOf('is-external=true') == -1) {<br>            parent.document.title="GZipCompressor (jbasejdbc   API)";<br>        }<br>    }<br>    catch(err) {<br>    }<br>//--><br>var methods = {"i0":10,"i1":10,"i2":10,"i3":10};<br>var tabs = {65535:["t0","All Methods"],2:["t2","Instance Methods"],8:["t4","Concrete Methods"]};<br>var altColor = "altColor";<br>var rowColor = "rowColor";<br>var tableTab = "tableTab";<br>var activeTableTab = "activeTableTab";
JavaScript is disabled on your browser.

Skip navigation links

- [Overview](../../../../overview-summary.html)
- [Package](./../com.jbase.jdbc.io-%28jbasejdbc---api%29)
- Class
- [Use](./../class-use/uses-of-class-com.jbase.jdbc.io.gzipcompressor-%28jbasejdbc---api%29)
- [Tree](./../com.jbase.jdbc.io-class-hierarchy-%28jbasejdbc---api%29)
- [Deprecated](../../../../deprecated-list.html)
- [Help](../../../../help-doc.html)


jbasejdbc <br>

- [Prev Class](./../errorresponse-%28jbasejdbc---api%29 "class in com.jbase.jdbc.io")
- [Next Class](./../ibyteobject-%28jbasejdbc---api%29 "interface in com.jbase.jdbc.io")


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

## Class GZipCompressor

- [java.lang.Object](http://java.sun.com/j2se/1.5.0/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang")
- - com.jbase.jdbc.io.GZipCompressor


- * * *


```
public class GZipCompressor
extends Object
```

- - ### Constructor Summary


Constructors | Constructor and Description |
| --- |
| `GZipCompressor()`  |


    - ### Method Summary


All Methods [Instance Methods](javascript:show%282%29;) [Concrete Methods](javascript:show%288%29;) | Modifier and Type | Method and Description |
| --- | --- |
| `byte[]` | `compress(byte[] data)`  |
| `byte[]` | `compress(byte[] data,<br>        int start,<br>        int sz)`  |
| `byte[]` | `uncompress(byte[] data)`  |
| `byte[]` | `uncompress(byte[] data,<br>          int start,<br>          int sz)`  |


        - ### Methods inherited from class java.lang.[Object](http://java.sun.com/j2se/1.5.0/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang")
`clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

- - ### Constructor Detail

        - #### GZipCompressor

```
public GZipCompressor()
```


    - ### Method Detail

        - #### compress

```
public byte[] compress(byte[] data)
                throws IOException
```
Throws:`IOException`


        - #### compress

```
public byte[] compress(byte[] data,
                       int start,
                       int sz)
                throws IOException
```
Throws:`IOException`


        - #### uncompress

```
public byte[] uncompress(byte[] data)
                  throws IOException
```
Throws:`IOException`


        - #### uncompress

```
public byte[] uncompress(byte[] data,
                         int start,
                         int sz)
                  throws IOException
```
Throws:`IOException`

Skip navigation links

- [Overview](../../../../overview-summary.html)
- [Package](./../com.jbase.jdbc.io-%28jbasejdbc---api%29)
- Class
- [Use](./../class-use/uses-of-class-com.jbase.jdbc.io.gzipcompressor-%28jbasejdbc---api%29)
- [Tree](./../com.jbase.jdbc.io-class-hierarchy-%28jbasejdbc---api%29)
- [Deprecated](../../../../deprecated-list.html)
- [Help](../../../../help-doc.html)


jbasejdbc <br>

- [Prev Class](./../errorresponse-%28jbasejdbc---api%29 "class in com.jbase.jdbc.io")
- [Next Class](./../ibyteobject-%28jbasejdbc---api%29 "interface in com.jbase.jdbc.io")


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
