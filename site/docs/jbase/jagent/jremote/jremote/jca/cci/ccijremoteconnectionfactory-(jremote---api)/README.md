# CCIJRemoteConnectionFactory (jremote   API)

**Created At:** 9/25/2017 11:54:36 AM  
**Updated At:** 2/15/2018 8:02:18 AM  
**Original Doc:** [com_jbase_jremote_jca_cci_CCIJRemoteConnectionFactory](https://docs.jbase.com/39259-cci/com_jbase_jremote_jca_cci_CCIJRemoteConnectionFactory)  

<!--<br>    try {<br>        if (location.href.indexOf('is-external=true') == -1) {<br>            parent.document.title="CCIJRemoteConnectionFactory (jremote   API)";<br>        }<br>    }<br>    catch(err) {<br>    }<br>//--><br>var methods = {"i0":10,"i1":10,"i2":10,"i3":10,"i4":10,"i5":10};<br>var tabs = {65535:["t0","All Methods"],2:["t2","Instance Methods"],8:["t4","Concrete Methods"]};<br>var altColor = "altColor";<br>var rowColor = "rowColor";<br>var tableTab = "tableTab";<br>var activeTableTab = "activeTableTab";
JavaScript is disabled on your browser.

Skip navigation links

- [Overview](../../../../../overview-summary.html)
- [Package](./../com.jbase.jremote.jca.cci-%28jremote---api%29)
- Class
- [Use](./../class-use/uses-of-class-com.jbase.jremote.jca.cci.ccijremoteconnectionfactory-%28jremote---api%29)
- [Tree](./../com.jbase.jremote.jca.cci-class-hierarchy-%28jremote---api%29)
- [Deprecated](../../../../../deprecated-list.html)
- [Help](../../../../../help-doc.html)


jremote <br>

- [Prev Class](./../ccijconnection-%28jremote---api%29 "class in com.jbase.jremote.jca.cci")
- [Next Class](./../ccijremotedynamicarrayrecord-%28jremote---api%29 "class in com.jbase.jremote.jca.cci")


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

com.jbase.jremote.jca.cci

## Class CCIJRemoteConnectionFactory

- [java.lang.Object](http://java.sun.com/j2se/1.5.0/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang")
- - com.jbase.jremote.jca.cci.CCIJRemoteConnectionFactory


- All Implemented Interfaces:[Serializable](http://java.sun.com/j2se/1.5.0/docs/api/java/io/Serializable.html?is-external=true "class or interface in java.io"), [Referenceable](http://java.sun.com/j2se/1.5.0/docs/api/javax/naming/Referenceable.html?is-external=true "class or interface in javax.naming"), javax.resource.cci.ConnectionFactory
* * *


```
public class CCIJRemoteConnectionFactory
extends Object
implements javax.resource.cci.ConnectionFactory
```
See Also:[Serialized Form](../../../../../serialized-form.html#com.jbase.jremote.jca.cci.CCIJRemoteConnectionFactory)

- - ### Field Summary


Fields | Modifier and Type | Field and Description |
| --- | --- |
| `protected javax.resource.cci.RecordFactory` | `_recordFactory`  |


    - ### Constructor Summary


Constructors | Constructor and Description |
| --- |
| `CCIJRemoteConnectionFactory()`<br>Construct a connection factory for use in a non managed environment using<br> the default connection manager.<br> |
| `CCIJRemoteConnectionFactory(javax.resource.spi.ManagedConnectionFactory mcf)`<br>Construct a connection factory for use in a non managed environment using<br> the default connection manager.<br> |
| `CCIJRemoteConnectionFactory(javax.resource.spi.ManagedConnectionFactory mcf,<br>                           javax.resource.spi.ConnectionManager cm)`<br>Constructor for managed connection factory.<br> |


    - ### Method Summary


All Methods [Instance Methods](javascript:show%282%29;) [Concrete Methods](javascript:show%288%29;) | Modifier and Type | Method and Description |
| --- | --- |
| `javax.resource.cci.Connection` | `getConnection()`  |
| `javax.resource.cci.Connection` | `getConnection(javax.resource.cci.ConnectionSpec cxSpec)`  |
| `javax.resource.cci.ResourceAdapterMetaData` | `getMetaData()`  |
| `javax.resource.cci.RecordFactory` | `getRecordFactory()`  |
| `Reference` | `getReference()`  |
| `void` | `setReference(Reference reference)`  |


        - ### Methods inherited from class java.lang.[Object](http://java.sun.com/j2se/1.5.0/docs/api/java/lang/Object.html?is-external=true "class or interface in java.lang")
`clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

- - ### Field Detail

        - #### \_recordFactory

```
protected javax.resource.cci.RecordFactory _recordFactory
```


    - ### Constructor Detail

        - #### CCIJRemoteConnectionFactory

```
public CCIJRemoteConnectionFactory()
```

Construct a connection factory for use in a non managed environment using<br> the default connection manager.
See Also:[`DefaultConnectionManager`](./../../defaultconnectionmanager-%28jremote-api%29 "class in com.jbase.jremote.jca")


        - #### CCIJRemoteConnectionFactory

```
public CCIJRemoteConnectionFactory(javax.resource.spi.ManagedConnectionFactory mcf)
```

Construct a connection factory for use in a non managed environment using<br> the default connection manager.
See Also:[`DefaultConnectionManager`](./../../defaultconnectionmanager-%28jremote-api%29 "class in com.jbase.jremote.jca")


        - #### CCIJRemoteConnectionFactory

```
public CCIJRemoteConnectionFactory(javax.resource.spi.ManagedConnectionFactory mcf,
                                   javax.resource.spi.ConnectionManager cm)
```

Constructor for managed connection factory.  The application server<br> will use this constructor and supply a configured ManagedConnectionFactory and<br> ConnectionManager.  This class will hook into the application server connection <br> pool via the supplied ConnectionManager.


    - ### Method Detail

        - #### getConnection

```
public javax.resource.cci.Connection getConnection()
                                            throws javax.resource.ResourceException
```
Specified by:`getConnection` in interface `javax.resource.cci.ConnectionFactory`Throws:`javax.resource.ResourceException`


        - #### getConnection

```
public javax.resource.cci.Connection getConnection(javax.resource.cci.ConnectionSpec cxSpec)
                                            throws javax.resource.ResourceException
```
Specified by:`getConnection` in interface `javax.resource.cci.ConnectionFactory`Throws:`javax.resource.ResourceException`


        - #### getMetaData

```
public javax.resource.cci.ResourceAdapterMetaData getMetaData()
                                                       throws javax.resource.ResourceException
```
Specified by:`getMetaData` in interface `javax.resource.cci.ConnectionFactory`Throws:`javax.resource.ResourceException`


        - #### getRecordFactory

```
public javax.resource.cci.RecordFactory getRecordFactory()
                                                  throws javax.resource.ResourceException
```
Specified by:`getRecordFactory` in interface `javax.resource.cci.ConnectionFactory`Throws:`javax.resource.ResourceException`


        - #### setReference

```
public void setReference(Reference reference)
```
See Also:`Referenceable.setReference(Reference)`


        - #### getReference

```
public Reference getReference()
                       throws NamingException
```
Specified by:`getReference` in interface `Referenceable`Throws:`NamingException`See Also:[`Referenceable.getReference()`](http://java.sun.com/j2se/1.5.0/docs/api/javax/naming/Referenceable.html?is-external=true#getReference-- "class or interface in javax.naming")

Skip navigation links

- [Overview](../../../../../overview-summary.html)
- [Package](./../com.jbase.jremote.jca.cci-%28jremote---api%29)
- Class
- [Use](./../class-use/uses-of-class-com.jbase.jremote.jca.cci.ccijremoteconnectionfactory-%28jremote---api%29)
- [Tree](./../com.jbase.jremote.jca.cci-class-hierarchy-%28jremote---api%29)
- [Deprecated](../../../../../deprecated-list.html)
- [Help](../../../../../help-doc.html)


jremote <br>

- [Prev Class](./../ccijconnection-%28jremote---api%29 "class in com.jbase.jremote.jca.cci")
- [Next Class](./../ccijremotedynamicarrayrecord-%28jremote---api%29 "class in com.jbase.jremote.jca.cci")


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
