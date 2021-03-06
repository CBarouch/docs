# Compile Introduction

**Created At:** 11/1/2017 12:21:45 AM  
**Updated At:** 11/1/2017 12:22:34 AM  
**Original Doc:** [compile-introduction](https://docs.jbase.com/44497-articles/compile-introduction)  
**Original ID:** 283761  
**Internal:** No  


The BASIC command is provided as a front end program to the jBASE jbc compiler. The jbc compiler converts the BASIC code into "C" and invokes the native "C" compiler to convert the "C" source code into a machine native object file.

```
BASIC BP PROGRAM1 SUB1
```

The BASIC command creates the object record as $PROGRAM1 in file BP. The BP file can be any file type supported by jBASE, whether it is a hashed file, directory and so on.

The steps used by BASIC command are as follows:

- Any supplied record keys with a dollar/pound prefix or a .o or .obj suffix are ignored.
- The source is moved to the current working directory as a temporary file called BASIC\_nn.c, where nn is the users port number.
- The source is compiled using the jbc command.
- The .o or .obj file is then moved back to the original source file with a dollar/pound prefix and the .o or .obj suffix removed.
- The command then cleans up any scratch files it created.


Note: If the original record key had a .b suffix then the .o or .objsuffix is not removed and the dollar/pound prefix not prepended.

A jBASE utility jCompileFile is available which invokes the BASIC compiler and produces an output and summary report, together with warnings and error lists. The syntax of jCompileFile is as follows:

```
jCompileFile -Options SourceFileName
```


| Option<br> | Description<br> |
| --- | --- |
| -p<br> | direct output and report to printer<br> |
| -v<br> | direct output and report to screen<br> |


The conversion report, output, warning lists and error lists are stored in the PortSave directory as jbc\_rep\_FileName, jbc\_out\_FileName,   jbc\_warn\_FileName and jbc\_err\_FileName respectively. The jbc\_err\_FileName can be used to create a select list to supply to [JED](https://https://static.zumasys.com/jbase/r99/knowledgebase/manuals/3.0/30manpages/man/ed2_jed.htm) to enable correction of errors or problems. If executed again the jCompileFile will only attempt to compile records in the jbc\_err\_FileName list else the jbc\_warn\_FileName if either list is not empty. e.g.

```
FORM-LIST PortSave jbc_err_FileName
JED FileName
jCompileFile -v FileName
```
