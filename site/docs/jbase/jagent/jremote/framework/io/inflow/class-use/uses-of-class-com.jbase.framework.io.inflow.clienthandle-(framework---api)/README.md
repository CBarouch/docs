# Uses of Class com.jbase.framework.io.inflow.ClientHandle (framework   API)

**Created At:** 9/25/2017 10:28:08 AM  
**Updated At:** 2/15/2018 8:02:41 AM  
**Original Doc:** [com_jbase_framework_io_inflow_class-use_ClientHandle](https://docs.jbase.com/39227-class-use/com_jbase_framework_io_inflow_class-use_ClientHandle)  
**Original ID:** 277753  
**Internal:** Yes  

<!--<br>    try {<br>        if (location.href.indexOf('is-external=true') == -1) {<br>            parent.document.title="Uses of Class com.jbase.framework.io.inflow.ClientHandle (framework   API)";<br>        }<br>    }<br>    catch(err) {<br>    }<br>//-->
JavaScript is disabled on your browser.

Skip navigation links

- [Overview](../../../../../../overview-summary.html)
- [Package](./../../com.jbase.framework.io.inflow-%28framework---api%29)
- [Class](./../../clienthandle-%28framework---api%29 "class in com.jbase.framework.io.inflow")
- Use
- [Tree](./../../com.jbase.framework.io.inflow-class-hierarchy-%28framework---api%29)
- [Deprecated](../../../../../../deprecated-list.html)
- [Help](../../../../../../help-doc.html)


framework <br>

- Prev
- Next


- [Frames](./.)
- [No Frames](./.)


- [All Classes](../../../../../../allclasses-noframe.html)


<!--<br>  allClassesLink = document.getElementById("allclasses\_navbar\_top");<br>  if(window==top) {<br>    allClassesLink.style.display = "block";<br>  }<br>  else {<br>    allClassesLink.style.display = "none";<br>  }<br>  //-->

## Uses of Class
com.jbase.framework.io.inflow.ClientHandle

- Packages that use [ClientHandle](./../../clienthandle-%28framework---api%29 "class in com.jbase.framework.io.inflow") | Package | Description |
| --- | --- |
| com.jbase.framework.io.inflow |   |
- - ### Uses of [ClientHandle](./../../clienthandle-%28framework---api%29 "class in com.jbase.framework.io.inflow") in [com.jbase.framework.io.inflow](./../../com.jbase.framework.io.inflow-%28framework---api%29)


Methods in [com.jbase.framework.io.inflow](./../../com.jbase.framework.io.inflow-%28framework---api%29) with parameters of type [ClientHandle](./../../clienthandle-%28framework---api%29 "class in com.jbase.framework.io.inflow") | Modifier and Type | Method and Description |
| --- | --- |
| `void` | RequestHandler.`handleClose(ClientHandle handle)`<br>Called when a client close event occurs.<br> |
| `byte[]` | RequestHandler.`handleRequest(ClientHandle handle,<br>             byte[] request)`<br>Called when a client has sent a request.<br> |
| `void` | RequestHandler.`handleResponse(ClientHandle handle,<br>              byte[] response)`<br>Send a response to the supplied client (sessionId).<br> |
| `void` | RequestHandler.`handleTimeout(ClientHandle handle)`<br>Called when a select times out waiting for client keys.<br> |

Skip navigation links

- [Overview](../../../../../../overview-summary.html)
- [Package](./../../com.jbase.framework.io.inflow-%28framework---api%29)
- [Class](./../../clienthandle-%28framework---api%29 "class in com.jbase.framework.io.inflow")
- Use
- [Tree](./../../com.jbase.framework.io.inflow-class-hierarchy-%28framework---api%29)
- [Deprecated](../../../../../../deprecated-list.html)
- [Help](../../../../../../help-doc.html)


framework <br>

- Prev
- Next


- [Frames](./.)
- [No Frames](./.)


- [All Classes](../../../../../../allclasses-noframe.html)


<!--<br>  allClassesLink = document.getElementById("allclasses\_navbar\_bottom");<br>  if(window==top) {<br>    allClassesLink.style.display = "block";<br>  }<br>  else {<br>    allClassesLink.style.display = "none";<br>  }<br>  //-->

*Copyright © 2017 jBASE, Inc.. All Rights Reserved.*
