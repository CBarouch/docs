# JConnectionCallbackHandler

**Created At:** 9/13/2017 7:55:03 PM  
**Updated At:** 9/13/2017 7:55:47 PM  
**Original Doc:** [jconnectioncallbackhandler](https://docs.jbase.com/39719-archive/jconnectioncallbackhandler)  
**Original ID:** 276693  
**Internal:** Yes  


## Interface JConnectionCallbackHandler

- ```
public interface JConnectionCallbackHandler
```
- - ### Method Summary


| Modifier and Type | Method and Description |
| --- | --- |
All Methods [Instance Methods](javascript%3Ashow%282%29;) [Abstract Methods](javascript%3Ashow%284%29;) | `boolean` | `initialise(Subject subject,           JConnection connection)` Initialise a connection for the supplied Subject.<br> |
| `boolean` | `reinitialise(Subject subject,             JConnection connection)` The Subject intends to use a connection that was previously  initialised for another Subject.<br> |
| `boolean` | `reuse(Subject subject,      JConnection connection)` The Subject is reusing the supplied connection.<br> |
- - ### Method Detail
 
        - #### initialise

```
boolean initialise(Subject subject,                    JConnection connection)
```

Initialise a connection for the supplied Subject.
    - - #### reuse

```
boolean reuse(Subject subject,               JConnection connection)
```

The Subject is reusing the supplied connection.
    - - #### reinitialise

```
boolean reinitialise(Subject subject,                      JConnection connection)
```

The Subject intends to use a connection that was previously  initialised for another Subject.

