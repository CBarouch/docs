# curlClose

Closes the designated ***curlHandle***, freeing its resources (and disconnecting any host connections).

## Synax:

***result_code*** = **curlClose**(***curlHandle***)

where:

| Variable | Type | Description |
|--|--|--|
***result_code*** | integer | an integer result code (0 for success)
***curlHandle*** | var | a [jCURL](../../jcurl) handle generated by [curlInit](../curlinit)
>Note: that curlHandles will be automatically cleaned up on program termination.

## Example
```
rc = curlInit(curlHandle)
... perform curl operations with curlHandle
rc = curlClose(curlHandle)
```