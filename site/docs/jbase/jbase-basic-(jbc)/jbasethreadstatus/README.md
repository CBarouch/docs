# JBASETHREADStatus

**Created At:** 9/14/2017 12:40:13 PM  
**Updated At:** 5/20/2019 5:35:05 PM  
**Original Doc:** [276769-jbasethreadstatus](https://docs.jbase.com/36868-jbase-basic/276769-jbasethreadstatus)  
**Original ID:** 276769  
**Internal:** No  

## Description

The **JBASETHREADStatus** command shows the status of all running threads.

It takes the general form:

```
JBASETHREADStatus(ThreadList)
```

Where:

**ThreadList** a list of all threads active in this process, with one attribute per thread.

The layout of the multi-values in each attribute is as follows:

- &lt; n,1 &gt; port number
- &lt; n,2 &gt; thread handle returned from [JBASETHREADCreate](./../jbasethreadcreate)

Example code can be found in the "Threads" folder under "samples" in the jBASE install directory.

Go back to [jBASE BASIC](./../jbase-basic-programmers-reference-guide).
