# PROGRAMMING NOTES

**Created At:** 9/26/2017 4:47:03 PM  
**Updated At:** 11/21/2017 3:30:11 AM  
**Original Doc:** [programming-notes](https://docs.zumasys.com/36577-mv-dashboard/programming-notes)  
**Original ID:** 278563  
**Internal:** No  


- Multiple widgets may be defined to call a single subroutine. The subroutine may use the G$WIDGET.NAME global variable to determine the name of the widget that is associated with the execution of the program.
- WIDGET.USER.DATA and GLOBAL.USER.DATA are stored and retrieved using MATWRITE and MATREAD statements. Therefore, you must not store attribute-mark delimited arrays in any of the associated dimensioned array positions.
- Widget programs must be designed to execute very quickly. Users may add several widgets to a single dashboard page, so it is important that the widgets run as fast as possible. Look at G$CALL.DUR to see the duration of each subroutine call. You must use the last widget in the dashboard to see the duration of each widget call before it.
- Widget programs must have no output to the screen. Any output generated by the widget programs can corrupt the HTTP response headers and the HTML structure.

