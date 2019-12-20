# STATUS Function

**Created At:** 9/27/2017 2:46:45 PM  
**Updated At:** 1/5/2018 6:02:32 PM  


# Usage: 

If used after an [OPENPATH](277542-openpath) statement, the **STATUS** function will find the cause of a file open failure (that is, for a statement in which the ELSE clause is used). The following values can be returned if the statement is unsuccessful:

For the file access commands, [READ](277646-read), [WRITE](279568-write), [OPEN](277537-open), the function returns:

- 0 if successful, or an
- Operating System error code if previous command failed.
- 13 is returned if permission denied on UNIX systems.




For [OCONV](277483-oconv) conversions, the function returns:

- 0 if conversion was successful,
- 1 if an invalid conversion is requested,
- 3 if conversion of possible invalid date.




If used after [CLOSE](266856-close), [DELETE](276025-delete), [MATREAD](276956-matread), [MATWRITE](276964-matwrite), [OPEN](277537-open), [READ](277646-read) or [WRITE](279568-write), **STATUS** returns 0 if successful and no error occurs. In the event an error occurs, status returns the error number.

If used after an [OPEN](277537-open), [OPENPATH](277542-openpath), or [OPENSEQ](277543-openseq) statement, the file type is returned if the file is opened successfully. If the file is not opened successfully, the following values may be returned:

If used after a [READ](277646-read) statement, the **STATUS**function returns, if the file is a distributed file, the following:

If used after a [READL](278657-readl), [READU](278774-readu), [READVL](278776-readvl), or [READVU](278777-readvu) statement, if the statement includes the LOCKED clause, the returned value is the terminal number, as returned by the WHO command, of the user who set the lock.

If used after a [READSEQ](278773-readseq) statement,

If used after a [READT](278662-readt), [REWIND](278788-rewind), [WEOF](279559-weof), or [WRITET](279572-writet) statement, the returned value is hardware-dependent (I.e. varies according to the characteristics of the specific tape drive unit). The documentation that accompanied drive unit for may offer information about interpreting the values returned by the **STATUS** function.



Go back to[jBASE BASIC](263498-jbase-basic).