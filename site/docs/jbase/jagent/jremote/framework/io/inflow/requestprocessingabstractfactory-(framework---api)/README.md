# RequestProcessingAbstractFactory (framework   API)

**Created At:** 9/25/2017 10:30:33 AM  
**Updated At:** 2/15/2018 8:02:35 AM  
**Original Doc:** [com_jbase_framework_io_inflow_RequestProcessingAbstractFactory](https://docs.jbase.com/39226-inflow/com_jbase_framework_io_inflow_RequestProcessingAbstractFactory)  

<!--<br>    try {<br>        if (location.href.indexOf('is-external=true') == -1) {<br>            parent.document.title="RequestProcessingAbstractFactory (framework   API)";<br>        }<br>    }<br>    catch(err) {<br>    }<br>//--><br>var methods = {"i0":6};<br>var tabs = {65535:["t0","All Methods"],2:["t2","Instance Methods"],4:["t3","Abstract Methods"]};<br>var altColor = "altColor";<br>var rowColor = "rowColor";<br>var tableTab = "tableTab";<br>var activeTableTab = "activeTableTab";
JavaScript is disabled on your browser.

Skip navigation links

- [Overview](../../../../../overview-summary.html)
- [Package](./../com.jbase.framework.io.inflow-%28framework---api%29)
- Class
- [Use](./../class-use/uses-of-interface-com.jbase.framework.io.inflow.requestprocessingabstractfactory-%28framework---api%29)
- [Tree](./../com.jbase.framework.io.inflow-class-hierarchy-%28framework---api%29)
- [Deprecated](../../../../../deprecated-list.html)
- [Help](../../../../../help-doc.html)


framework <br>

- [Prev Class](./../requestlistenerthread-%28framework---api%29 "class in com.jbase.framework.io.inflow")
- [Next Class](./../statisticscounter-%28framework---api%29 "interface in com.jbase.framework.io.inflow")


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

com.jbase.framework.io.inflow

## Interface RequestProcessingAbstractFactory

- * * *


```
public interface RequestProcessingAbstractFactory
```

- - ### Method Summary


All Methods [Instance Methods](javascript:show%282%29;) [Abstract Methods](javascript:show%284%29;) | Modifier and Type | Method and Description |
| --- | --- |
| `RequestHandler` | `createRequestHandler(RequestListenerService rls)`<br>In ThreadPerConnection mode this method will be called by<br> RequestListenerService when new connection is opened.<br> |

- - ### Method Detail

        - #### createRequestHandler

```
RequestHandler createRequestHandler(RequestListenerService rls)
```

In ThreadPerConnection mode this method will be called by<br> RequestListenerService when new connection is opened.  This creates<br> one RequestHandler for each connection.
Parameters:`rls` - Returns:RequestHandler instance

Skip navigation links

- [Overview](../../../../../overview-summary.html)
- [Package](./../com.jbase.framework.io.inflow-%28framework---api%29)
- Class
- [Use](./../class-use/uses-of-interface-com.jbase.framework.io.inflow.requestprocessingabstractfactory-%28framework---api%29)
- [Tree](./../com.jbase.framework.io.inflow-class-hierarchy-%28framework---api%29)
- [Deprecated](../../../../../deprecated-list.html)
- [Help](../../../../../help-doc.html)


framework <br>

- [Prev Class](./../requestlistenerthread-%28framework---api%29 "class in com.jbase.framework.io.inflow")
- [Next Class](./../statisticscounter-%28framework---api%29 "interface in com.jbase.framework.io.inflow")


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
