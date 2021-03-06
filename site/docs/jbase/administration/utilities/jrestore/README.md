# jrestore

**Created At:** 7/20/2018 2:49:29 PM  
**Updated At:** 11/8/2019 8:35:07 AM  
**Original Doc:** [jrestore](https://docs.jbase.com/46963-utilities/jrestore)  
**Original ID:** 328719  
**Internal:** No  

**Tags:**
<badge text='recovery' vertical='middle' />
<badge text='restore' vertical='middle' />
<badge text='jrestore' vertical='middle' />
<badge text='file recovery' vertical='middle' />
<badge text='backup' vertical='middle' />
<badge text='file maintenance' vertical='middle' />

## Description 

The jrestore utility provides fast on-line restores from the saves produced by the [jbackup](./../jbackup) utility.

The jrestore can be controlled to restore from any file type on the backup, from single records to multiple directories.

The jrestore utility can also be used to verify jbackup saves.

```
jrestore -Options
```

where options may be:

-


| Option<br> | Explanation<br> |
| --- | --- |
| -a<br> | restore from current media position<br> |
| -bn<br> | set number of read buffers to n (default is 8, minimum is 1)<br> |
| -c"old new"<br> | restore old directory path as new directory path<br> |
| -d"DirRE"<br> | restore directory files matching regular expression<br> |
| -f Device<br> | restore from device file, default stdin<br> |
| -h"HashRE"<br> | restore hash files matching regular expression<br> |
| -H FileList<br> | restore files using only file names from FileList file<br> |
| -i"ItemRE"<br> | restore hash file items matching regular expression<br> |
| -I ItemList<br> | restore hash file items using only item ids from ItemList file<br> |
| -l"LnkdRE"<br> | restore links matching regular expression<br> |
| -k EncKey<br> | Encryption key<br> |
| -n<br> | control info files not restored<br> |
| -N<br> | control info files restored and indexes rebuilt<br> |
| -o"OfileRE"<br> | restore other files matching regular expression<br> |
| -pn<br> | set priority, nice value of parent process<br> |
| -u"UfileRE"<br> | restore normal file matching regular expression<br> |
| -v<br> | verbose mode<br> |
| -F<br> | use fixed block device. Use for QIC tapes<br> |
| -B<br> | force block size to 128k, default 16k<br> |
| -Cn<br> | force block size to n bytes, rounded to nearest k<br> |
| -P<br> | print and scan files only, no restore<br> |
| -O<br> | overwrite existing files and records<br> |
| -R<br> | suppress rewind last reel<br> |
| -T type<br> | restore hash files as specified file type; the original modulo and separation will be retained rather than use the 'resize' parameters.<br> |
| -U<br> | update only does not overwrite existing files or records<br> |
| -V<br> | verbose dot mode, displays a "." for each file<br> |
| -W | Roll forware TJ logfiles after database restore<br> |
| -X | Clear existing hashed files b efore population |
| -Z"RegExp"<br>(jBASE 5.8) | All-encompassing option that allows anything to be restored.<br>It is similar to: -u"regexp" -h"regexp" -d"regexp" -o"regexp" -l"regexp"<br>This option can be specified more than once on the command line.<br> |




When using jrestore, ensure that the command is executed at the standard shell not in jsh otherwise the double quotes and other meta characters will lose their meaning.



## Note: 


> On Windows, when specifying Windows path names the backslash must be escaped with a backslash, otherwise the backslash character is removed. e.g.
> 
> ```
> C:\\MyApp\\new
> ```




Examples of use may be as:

```
jrestore -f /dev/rmt/ctape -P
```

Reads formatted files and directories from a streaming cartridge device, displaying each file or directory as it is encountered.

This option can be used to verify that the tape does not contain any parity or formatting errors and so can be restored at a later date.

```
jrestore -f /dev/rmt/floppy -v
```

Reads and restores formatted files and directories from a floppy disk device, displaying each file or directory as it is encountered.

```
jbackup -Ajbase | jrestore -c"/home/old /home/new"
```

Reads formatted files and directories from stdin, which is being supplied by jbackup, modifies all occurrences of path string /home/old to /home/new and then restores files and directories using modified path string.

```
jrestore -f BACKUP -d".*PAYROLL$"
```

Reads formatted files and directories from UNIX file BACKUP, limits restore to any directories whose path name ends in PAYROLL.

```
jrestore -f BACKUP -h"/CUSTOMERS$" -i".*SMITH.*"
```

Reads formatted files and directories from UNIX file BACKUP, limits restore to any hash files whose path name ends in CUSTOMERS, and only restores record ids containing the string SMITH.
