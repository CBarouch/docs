# UnexpectedCharacterException (jbasejdbc   API)

**Created At:** 9/25/2017 10:49:09 AM  
**Updated At:** 2/15/2018 8:02:50 AM  
**Original Doc:** [com_jbase_jdbc_io_exception_UnexpectedCharacterException](https://docs.jbase.com/39236-exception/com_jbase_jdbc_io_exception_UnexpectedCharacterException)  
**Original ID:** 277869  
**Internal:** Yes  

<!--<br>    try {<br>        if (location.href.indexOf('is-external=true') == -1) {<br>            parent.document.title="UnexpectedCharacterException (jbasejdbc   API)";<br>        }<br>    }<br>    catch(err) {<br>    }<br>//-->
JavaScript is disabled on your browser.

Skip navigation links

- [Overview](../../../../../overview-summary.html)
- [Package](./../com.jbase.jdbc.io.exception-%28jbasejdbc---api%29)
- Class
- [Use](./../class-use/uses-of-class-com.jbase.jdbc.io.exception.unexpectedcharacterexception-%28jbasejdbc---api%29)
- [Tree](./../com.jbase.jdbc.io.exception-class-hierarchy-%28jbasejdbc---api%29)
- [Deprecated](../../../../../deprecated-list.html)
- [Help](../../../../../help-doc.html)


jbasejdbc <br>

- Prev Class
- [Next Class](./../unknowntypeexception-%28jbasejdbc---api%29 "class in com.jbase.jdbc.io.exception")


- [Frames](./.)
- [No Frames](./.)


- [All Classes](../../../../../allclasses-noframe.html)


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

com.jbase.jdbc.io.exception

## Class UnexpectedCharacterException

- [java.lang.Object](http://java.sun.com/j2se/1.5.0/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang")
- - [java.lang.Throwable](http://java.sun.com/j2se/1.5.0/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang")
    - - [java.lang.Exception](http://java.sun.com/j2se/1.5.0/docs/api/java/lang/Exception.html?is-external=true "class or interface in java.lang")
        - - [java.io.IOException](http://java.sun.com/j2se/1.5.0/docs/api/java/io/IOException.html?is-external=true "class or interface in java.io")
            - - com.jbase.jdbc.io.exception.UnexpectedCharacterException


- All Implemented Interfaces:[Serializable](http://java.sun.com/j2se/1.5.0/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io")
* * *


```
public class UnexpectedCharacterException
extends IOException
```
See Also:[Serialized Form](./../../../../jrcs/serialized-form#com.jbase.jdbc.io.exception)

- - ### Field Summary


Fields | Modifier and Type | Field and Description |
| --- | --- |
| `char` | `theChar`  |


    - ### Constructor Summary


Constructors | Constructor and Description |
| --- |
| `UnexpectedCharacterException(char c)`  |


    - ### Method Summary

        - ### Methods inherited from class java.lang.[Throwable](http://java.sun.com/j2se/1.5.0/docs/api/java/lang/Throwable.html?is-external=true "class or interface in java.lang")
`addSuppressed, fillInStackTrace, getCause, getLocalizedMessage, getMessage, getStackTrace, getSuppressed, initCause, printStackTrace, printStackTrace, printStackTrace, setStackTrace, toString`


        - ### Methods inherited from class java.lang.[Object](http://java.sun.com/j2se/1.5.0/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang")
`clone, equals, finalize, getClass, hashCode, notify, notifyAll, wait, wait, wait`

- - ### Field Detail

        - #### theChar

```
public char theChar
```


    - ### Constructor Detail

        - #### UnexpectedCharacterException

```
public UnexpectedCharacterException(char c)
```

Skip navigation links

- [Overview](../../../../../overview-summary.html)
- [Package](./../com.jbase.jdbc.io.exception-%28jbasejdbc---api%29)
- Class
- [Use](./../class-use/uses-of-class-com.jbase.jdbc.io.exception.unexpectedcharacterexception-%28jbasejdbc---api%29)
- [Tree](./../com.jbase.jdbc.io.exception-class-hierarchy-%28jbasejdbc---api%29)
- [Deprecated](../../../../../deprecated-list.html)
- [Help](../../../../../help-doc.html)


jbasejdbc <br>

- Prev Class
- [Next Class](./../unknowntypeexception-%28jbasejdbc---api%29 "class in com.jbase.jdbc.io.exception")


- [Frames](./.)
- [No Frames](./.)


- [All Classes](../../../../../allclasses-noframe.html)


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
