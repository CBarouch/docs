# ClientHandle (jremote   API)

**Created At:** 9/25/2017 11:49:36 AM  
**Updated At:** 2/15/2018 8:02:46 AM  
**Original Doc:** [com_jbase_jremote_io_inflow_ClientHandle](https://docs.jbase.com/39256-inflow/com_jbase_jremote_io_inflow_ClientHandle)  
**Original ID:** 278139  
**Internal:** Yes  

<!--<br>    try {<br>        if (location.href.indexOf('is-external=true') == -1) {<br>            parent.document.title="ClientHandle (jremote   API)";<br>        }<br>    }<br>    catch(err) {<br>    }<br>//--><br>var methods = {"i0":10,"i1":10,"i2":10};<br>var tabs = {65535:["t0","All Methods"],2:["t2","Instance Methods"],8:["t4","Concrete Methods"]};<br>var altColor = "altColor";<br>var rowColor = "rowColor";<br>var tableTab = "tableTab";<br>var activeTableTab = "activeTableTab";
JavaScript is disabled on your browser.

Skip navigation links

- [Overview](../../../../../overview-summary.html)
- [Package](./../com.jbase.jremote.io.inflow-%28jremote---api%29)
- Class
- [Use](./../class-use/uses-of-class-com.jbase.jremote.io.inflow.clienthandle-%28jremote---api%29)
- [Tree](./../com.jbase.jremote.io.inflow-class-hierarchy-%28jremote---api%29)
- [Deprecated](../../../../../deprecated-list.html)
- [Help](../../../../../help-doc.html)


jremote <br>

- Prev Class
- [Next Class](./../pendingchange-%28jremote---api%29 "class in com.jbase.jremote.io.inflow")


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

com.jbase.jremote.io.inflow

## Class ClientHandle

- [java.lang.Object](http://java.sun.com/j2se/1.5.0/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang")
- - com.jbase.jremote.io.inflow.ClientHandle


- * * *


```
public class ClientHandle
extends Object
```

This class holds a reference to the object the RequestServiceListener<br> uses to send reponses to clients.  This object can be either a SocketChannel<br> or a Socket.
Author:aphethean

- - ### Field Summary


Fields | Modifier and Type | Field and Description |
| --- | --- |
| `SocketChannel` | `_channel`  |
| `Socket` | `_socket`  |


    - ### Constructor Summary


Constructors | Constructor and Description |
| --- |
| `ClientHandle(Socket s)`<br>Java 1.4 IO should create a response handler with the socket.<br> |
| `ClientHandle(SocketChannel c)`<br>Java NIO (5 and above) is capable of more advanced response handling<br> and should use this constructor.<br> |


    - ### Method Summary


All Methods [Instance Methods](javascript:show%282%29;) [Concrete Methods](javascript:show%288%29;) | Modifier and Type | Method and Description |
| --- | --- |
| `SocketChannel` | `getChannel()`  |
| `String` | `getSessionId()`  |
| `Socket` | `getSocket()`  |


        - ### Methods inherited from class java.lang.[Object](http://java.sun.com/j2se/1.5.0/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang")
`clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

- - ### Field Detail

        - #### \_channel

```
public SocketChannel _channel
```


        - #### \_socket

```
public Socket _socket
```


    - ### Constructor Detail

        - #### ClientHandle

```
public ClientHandle(SocketChannel c)
```

Java NIO (5 and above) is capable of more advanced response handling<br> and should use this constructor.
Parameters:`c` -


        - #### ClientHandle

```
public ClientHandle(Socket s)
```

Java 1.4 IO should create a response handler with the socket.
Parameters:`s` -


    - ### Method Detail

        - #### getSessionId

```
public String getSessionId()
```


        - #### getChannel

```
public SocketChannel getChannel()
```


        - #### getSocket

```
public Socket getSocket()
```

Skip navigation links

- [Overview](../../../../../overview-summary.html)
- [Package](./../com.jbase.jremote.io.inflow-%28jremote---api%29)
- Class
- [Use](./../class-use/uses-of-class-com.jbase.jremote.io.inflow.clienthandle-%28jremote---api%29)
- [Tree](./../com.jbase.jremote.io.inflow-class-hierarchy-%28jremote---api%29)
- [Deprecated](../../../../../deprecated-list.html)
- [Help](../../../../../help-doc.html)


jremote <br>

- Prev Class
- [Next Class](./../pendingchange-%28jremote---api%29 "class in com.jbase.jremote.io.inflow")


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
