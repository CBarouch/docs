# JRemoteRequestProcessingFactory (jremote   API)

**Created At:** 9/25/2017 12:05:48 PM  
**Updated At:** 2/15/2018 8:02:55 AM  
**Original Doc:** [com_jbase_jremote_jca_JRemoteRequestProcessingFactory](https://docs.jbase.com/39258-jca/com_jbase_jremote_jca_JRemoteRequestProcessingFactory)  
**Original ID:** 278271  
**Internal:** Yes  

<!--<br>    try {<br>        if (location.href.indexOf('is-external=true') == -1) {<br>            parent.document.title="JRemoteRequestProcessingFactory (jremote   API)";<br>        }<br>    }<br>    catch(err) {<br>    }<br>//--><br>var methods = {"i0":10};<br>var tabs = {65535:["t0","All Methods"],2:["t2","Instance Methods"],8:["t4","Concrete Methods"]};<br>var altColor = "altColor";<br>var rowColor = "rowColor";<br>var tableTab = "tableTab";<br>var activeTableTab = "activeTableTab";
JavaScript is disabled on your browser.

Skip navigation links

- [Overview](../../../../overview-summary.html)
- [Package](./../com.jbase.jremote.jca-%28jremote---api%29)
- Class
- [Use](./../class-use/uses-of-class-com.jbase.jremote.jca.jremoterequestprocessingfactory-%28jremote---api%29)
- [Tree](./../com.jbase.jremote.jca-class-hierarchy-%28jremote---api%29)
- [Deprecated](../../../../deprecated-list.html)
- [Help](../../../../help-doc.html)


jremote <br>

- [Prev Class](./../jremotemanagedconnectionmetadata-%28jremote---api%29 "class in com.jbase.jremote.jca")
- [Next Class](./../jremoteresourceadapter-%28jremote-api%29 "class in com.jbase.jremote.jca")


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

com.jbase.jremote.jca

## Class JRemoteRequestProcessingFactory

- [java.lang.Object](http://java.sun.com/j2se/1.5.0/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang")
- - com.jbase.jremote.jca.JRemoteRequestProcessingFactory


- All Implemented Interfaces:[RequestProcessingAbstractFactory](./../../io/inflow/requestprocessingabstractfactory-%28jremote---api%29 "interface in com.jbase.jremote.io.inflow")
* * *


```
public class JRemoteRequestProcessingFactory
extends Object
implements RequestProcessingAbstractFactory
```

- - ### Constructor Summary


Constructors | Constructor and Description |
| --- |
| `JRemoteRequestProcessingFactory(List<EndpointAdapter> eps)`  |


    - ### Method Summary


All Methods [Instance Methods](javascript:show%282%29;) [Concrete Methods](javascript:show%288%29;) | Modifier and Type | Method and Description |
| --- | --- |
| `RequestHandler` | `createRequestHandler(RequestListenerService rls)`<br>In ThreadPerConnection mode this method will be called by<br> RequestListenerService when new connection is opened.<br> |


        - ### Methods inherited from class java.lang.[Object](http://java.sun.com/j2se/1.5.0/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang")
`clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

- - ### Constructor Detail

        - #### JRemoteRequestProcessingFactory

```
public JRemoteRequestProcessingFactory(List<EndpointAdapter> eps)
```


    - ### Method Detail

        - #### createRequestHandler

```
public RequestHandler createRequestHandler(RequestListenerService rls)
```

Description copied from interface: `RequestProcessingAbstractFactory`

In ThreadPerConnection mode this method will be called by<br> RequestListenerService when new connection is opened.  This creates<br> one RequestHandler for each connection.
Specified by:`createRequestHandler` in interface `RequestProcessingAbstractFactory`Returns:RequestHandler instance

Skip navigation links

- [Overview](../../../../overview-summary.html)
- [Package](./../com.jbase.jremote.jca-%28jremote---api%29)
- Class
- [Use](./../class-use/uses-of-class-com.jbase.jremote.jca.jremoterequestprocessingfactory-%28jremote---api%29)
- [Tree](./../com.jbase.jremote.jca-class-hierarchy-%28jremote---api%29)
- [Deprecated](../../../../deprecated-list.html)
- [Help](../../../../help-doc.html)


jremote <br>

- [Prev Class](./../jremotemanagedconnectionmetadata-%28jremote---api%29 "class in com.jbase.jremote.jca")
- [Next Class](./../jremoteresourceadapter-%28jremote-api%29 "class in com.jbase.jremote.jca")


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
