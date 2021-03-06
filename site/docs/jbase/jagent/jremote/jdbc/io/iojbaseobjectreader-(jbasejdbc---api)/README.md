# IOJBaseObjectReader (jbasejdbc   API)

**Created At:** 9/25/2017 10:52:14 AM  
**Updated At:** 2/15/2018 8:02:51 AM  
**Original Doc:** [com_jbase_jdbc_io_IOJBaseObjectReader](https://docs.jbase.com/39232-io/com_jbase_jdbc_io_IOJBaseObjectReader)  
**Original ID:** 277894  
**Internal:** Yes  

<!--<br>    try {<br>        if (location.href.indexOf('is-external=true') == -1) {<br>            parent.document.title="IOJBaseObjectReader (jbasejdbc   API)";<br>        }<br>    }<br>    catch(err) {<br>    }<br>//--><br>var methods = {"i0":10,"i1":10,"i2":10,"i3":10,"i4":10,"i5":10,"i6":10,"i7":10,"i8":10,"i9":10,"i10":10,"i11":10};<br>var tabs = {65535:["t0","All Methods"],2:["t2","Instance Methods"],8:["t4","Concrete Methods"]};<br>var altColor = "altColor";<br>var rowColor = "rowColor";<br>var tableTab = "tableTab";<br>var activeTableTab = "activeTableTab";
JavaScript is disabled on your browser.

Skip navigation links

- [Overview](../../../../overview-summary.html)
- [Package](./../com.jbase.jdbc.io-%28jbasejdbc---api%29)
- Class
- [Use](./../class-use/uses-of-class-com.jbase.jdbc.io.iojbaseobjectreader-%28jbasejdbc---api%29)
- [Tree](./../com.jbase.jdbc.io-class-hierarchy-%28jbasejdbc---api%29)
- [Deprecated](../../../../deprecated-list.html)
- [Help](../../../../help-doc.html)


jbasejdbc <br>

- [Prev Class](./../ibyteobject-%28jbasejdbc---api%29 "interface in com.jbase.jdbc.io")
- [Next Class](./../iojbaseobjectwriter-%28jbasejdbc---api%29 "class in com.jbase.jdbc.io")


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

## Class IOJBaseObjectReader

- [java.lang.Object](http://java.sun.com/j2se/1.5.0/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang")
- - [com.jbase.jdbc.io.AbstractJBaseObjectReader](./../abstractjbaseobjectreader-%28jbasejdbc---api%29 "class in com.jbase.jdbc.io")
    - - com.jbase.jdbc.io.IOJBaseObjectReader


- All Implemented Interfaces:[JBaseObjectReader](./../jbaseobjectreader-%28jbasejdbc-api%29 "interface in com.jbase.jdbc.io")
* * *


```
public class IOJBaseObjectReader
extends AbstractJBaseObjectReader
```

jBase object reader based on the DataInputStream.
Author:aphethean

- - ### Field Summary

        - ### Fields inherited from class com.jbase.jdbc.io.[AbstractJBaseObjectReader](./../abstractjbaseobjectreader-%28jbasejdbc---api%29 "class in com.jbase.jdbc.io")
`log`


    - ### Constructor Summary


Constructors | Modifier | Constructor and Description |
| --- | --- |
| `protected` | `IOJBaseObjectReader()`  |
| `` | `IOJBaseObjectReader(ObjectFactory factory,<br>                   byte[] b)`<br>Constructor FOR TESTING ONLY.<br> |
| `` | `IOJBaseObjectReader(ObjectFactory factory,<br>                   InputStream is)`  |


    - ### Method Summary


All Methods [Instance Methods](javascript:show%282%29;) [Concrete Methods](javascript:show%288%29;) | Modifier and Type | Method and Description |
| --- | --- |
| `protected int` | `bufferedRead()`  |
| `void` | `close()`  |
| `protected byte` | `getByte()`  |
| `protected int` | `getBytes(byte[] buf)`  |
| `protected int` | `getBytes(ByteBuffer bBuf)`  |
| `protected int` | `getInt()`  |
| `ObjectFactory` | `getObjectFactory()`<br>This method must be implemented by concrete ObjectReaders.<br> |
| `protected int` | `inBytes(int numberOfBytesToRead)`  |
| `protected boolean` | `isClosed()`  |
| `boolean` | `isUnpackRequired()`  |
| `protected String` | `readUTF()`  |
| `void` | `unpack()`  |


        - ### Methods inherited from class com.jbase.jdbc.io.[AbstractJBaseObjectReader](./../abstractjbaseobjectreader-%28jbasejdbc---api%29 "class in com.jbase.jdbc.io")
`checkBuffer, readByteObject, readBytes, readInt, readJBaseSerializableObject, readObject, readObject, readObject, readRootObject, readString`


        - ### Methods inherited from class java.lang.[Object](http://java.sun.com/j2se/1.5.0/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang")
`clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

- - ### Constructor Detail

        - #### IOJBaseObjectReader

```
protected IOJBaseObjectReader()
```


        - #### IOJBaseObjectReader

```
public IOJBaseObjectReader(ObjectFactory factory,
                           InputStream is)
```


        - #### IOJBaseObjectReader

```
public IOJBaseObjectReader(ObjectFactory factory,
                           byte[] b)
```

Constructor FOR TESTING ONLY. Constructe the buffer and writes the info<br> passed into it. i.e. simulates this data arriving over the wire.


    - ### Method Detail

        - #### getObjectFactory

```
public ObjectFactory getObjectFactory()
```

Description copied from class: `AbstractJBaseObjectReader`

This method must be implemented by concrete ObjectReaders.
Specified by:`getObjectFactory` in class `AbstractJBaseObjectReader`Returns:an instance of a class implementing JBaseSerializable


        - #### close

```
public void close()
           throws IOException
```
Specified by:`close` in interface `JBaseObjectReader`Specified by:`close` in class `AbstractJBaseObjectReader`Throws:`IOException`


        - #### getByte

```
protected byte getByte()
                throws IOException
```
Specified by:`getByte` in class `AbstractJBaseObjectReader`Throws:`IOException`


        - #### getInt

```
protected int getInt()
              throws IOException
```
Specified by:`getInt` in class `AbstractJBaseObjectReader`Throws:`IOException`


        - #### getBytes

```
protected int getBytes(byte[] buf)
                throws IOException
```
Specified by:`getBytes` in class `AbstractJBaseObjectReader`Throws:`IOException`


        - #### getBytes

```
protected int getBytes(ByteBuffer bBuf)
                throws IOException
```
Specified by:`getBytes` in class `AbstractJBaseObjectReader`Throws:`IOException`


        - #### readUTF

```
protected String readUTF()
                  throws IOException
```
Specified by:`readUTF` in class `AbstractJBaseObjectReader`Throws:`IOException`


        - #### inBytes

```
protected int inBytes(int numberOfBytesToRead)
               throws IOException
```
Specified by:`inBytes` in class `AbstractJBaseObjectReader`Throws:`IOException`


        - #### isClosed

```
protected boolean isClosed()
```


        - #### bufferedRead

```
protected int bufferedRead()
                    throws IOException
```
Overrides:`bufferedRead` in class `AbstractJBaseObjectReader`Throws:`IOException`


        - #### unpack

```
public void unpack()
            throws IOException
```
Throws:`IOException`


        - #### isUnpackRequired

```
public boolean isUnpackRequired()
                         throws IOException
```
Throws:`IOException`

Skip navigation links

- [Overview](../../../../overview-summary.html)
- [Package](./../com.jbase.jdbc.io-%28jbasejdbc---api%29)
- Class
- [Use](./../class-use/uses-of-class-com.jbase.jdbc.io.iojbaseobjectreader-%28jbasejdbc---api%29)
- [Tree](./../com.jbase.jdbc.io-class-hierarchy-%28jbasejdbc---api%29)
- [Deprecated](../../../../deprecated-list.html)
- [Help](../../../../help-doc.html)


jbasejdbc <br>

- [Prev Class](./../ibyteobject-%28jbasejdbc---api%29 "interface in com.jbase.jdbc.io")
- [Next Class](./../iojbaseobjectwriter-%28jbasejdbc---api%29 "class in com.jbase.jdbc.io")


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
