# Method: $prepend()

**Created At:** 2/15/2018 2:58:49 PM  
**Updated At:** 2/11/2019 8:50:15 AM  
**Original Doc:** [method-prepend](https://docs.jbase.com/42948-dynamic-objects/method-prepend)  
**Original ID:** 299339  
**Internal:** No  


## Description

The **$prepend()** method allows you to insert a new value at the beginning of the array.



## Syntax

```
arr->$prepend(value(,reject_duplicates{,case_insensitive}}
```



## Arguments




| <!----> | <!----> |
| --- | --- |
| Argument<br> | Description<br> |
| value<br> | the value to prepend<br> |
| reject\_duplicates | 0 = Duplicates are allowed (default)<br>1 = Duplicates are rejected |
| case\_insensitive | 0 = The duplicate check is case sensitive (default)<br>1 = The duplicate check is case insensitive (any non-zero number is valid) |




## Return value

The current array



## Examples

```
json = \["two","three","four"]\
crt "Initial array: ":json
jarray = json->$fromjson()
jarray->$prepend("one")->$prepend("zero")
crt jarray->$tojson()
```

Result:

```
Initial array: ["two","three","four"]
["zero","one","two","three","four"]
```



## Notes

See also [$append()](./../method-$append%28%29)
