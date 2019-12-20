# JStatementImpl (jremote API)

**Created At:** 9/25/2017 11:52:59 AM  
**Updated At:** 12/24/2018 8:55:27 PM  

<!--<br>    try {<br>        if (location.href.indexOf('is-external=true') == -1) {<br>            parent.document.title="JStatementImpl (jremote   API)";<br>        }<br>    }<br>    catch(err) {<br>    }<br>//--><br>var methods = {"i0":10,"i1":10,"i2":10,"i3":10,"i4":10};<br>var tabs = {65535:["t0","All Methods"],2:["t2","Instance Methods"],8:["t4","Concrete Methods"]};<br>var altColor = "altColor";<br>var rowColor = "rowColor";<br>var tableTab = "tableTab";<br>var activeTableTab = "activeTableTab";


## Class JStatementImpl

All Implemented Interfaces:[JStatement](/39248-jremote/com_jbase_jremote_JStatement "interface in com.jbase.jremote")
* * *


```
public class JStatementImpl
extends Object
implements JStatement
```

### Constructor Summary


| Constructor and Description<br> |
| --- |
| `JStatementImpl(AbstractJRemoteConnection connection)`<br>Constructor.<br> |






### Method Summary


| Modifier and Type<br> | Method and Description<br> |
| --- | --- |
| `JResultSet`<br> | `execute(JDynArray queries)`<br>Execute query.<br> |
| `JResultSet`<br> | `execute(JDynArray queries, JSelectList selectList)`<br>Execute query using an existing select list as a filter.<br> |
| `JResultSet`<br> | `execute(String query)`<br>Execute query.<br> |
| `JResultSet`<br> | `execute(String query, JSelectList selectList)`<br>Execute query using an existing select list as a filter.<br> |
| `void`<br> | `setFetchSize(int rows)`<br>Sets the fetch size.<br> |


- Methods inherited from class java.lang.Object
    - `clone, equals, finalize, getClass, hashCode, notify, notifyAll, toString, wait, wait, wait`

### Constructor Detail

#### JStatementImpl

```
public JStatementImpl(AbstractJRemoteConnection connection)
```

Constructor.
Parameters:`connection` -






### Method Detail

#### execute

```
public JResultSet execute(String query)
                   throws JRemoteException
```

Description copied from interface: `JStatement`

Execute query.
Specified by:`execute` in interface `JStatement`Parameters:`query` - as a stringReturns:result setThrows:`JRemoteException`See Also:[`JStatement.execute(java.lang.String)`](/39248-jremote/com_jbase_jremote_JStatement#execute-java.lang.String-)


#### execute

```
public JResultSet execute(JDynArray queries)
                   throws JRemoteException
```

Description copied from interface: `JStatement`

Execute query.
Specified by:`execute` in interface `JStatement`Parameters:`queries` - query as a dynamic arrayReturns:result setThrows:`JRemoteException`See Also:[`JStatement.execute(com.jbase.jremote.JDynArray)`](/39248-jremote/com_jbase_jremote_JStatement#execute-com.jbase.jremote.JDynArray-)

#### execute

```
public JResultSet execute(String query,
                          JSelectList selectList)
                   throws JRemoteException
```

Description copied from interface: `JStatement`

Execute query using an existing select list as a filter.
Specified by:`execute` in interface `JStatement`Parameters:`query` - as a stringReturns:result setThrows:`JRemoteException`See Also:[`JStatement.execute(java.lang.String, com.jbase.jremote.JSelectList)`](/39248-jremote/com_jbase_jremote_JStatement#execute-java.lang.String-com.jbase.jremote.JSelectList-)
#### execute

```
public JResultSet execute(JDynArray queries,
                          JSelectList selectList)
                   throws JRemoteException
```

Description copied from interface: `JStatement`

Execute query using an existing select list as a filter.
Specified by:`execute` in interface `JStatement`Parameters:`queries` - query as a dynamic arrayReturns:result setThrows:`JRemoteException`See Also:[`JStatement.execute(com.jbase.jremote.JDynArray, com.jbase.jremote.JSelectList)`](/39248-jremote/com_jbase_jremote_JStatement#execute-com.jbase.jremote.JDynArray-com.jbase.jremote.JSelectList-)


#### setFetchSize

```
public void setFetchSize(int rows)
```

Description copied from interface: `JStatement`

Sets the fetch size.
Specified by:`setFetchSize` in interface `JStatement`See Also:[`JStatement.setFetchSize(int)`](/39248-jremote/com_jbase_jremote_JStatement#setFetchSize-int-)

Back to [jREMOTE API](com_jbase_jremote_package-summary)

