Why would you want to call a third party API on the FRONTEND instead of the back end.  See Schemes A and B below. 

Evaluation: 2 valid answers satisfy this question though more answers are possible.

Scheme A (Client making 3rd party HTTP call):
```
 /---------                |----------|
|          |  http calls   |          |
|  browser | ------------> |    my    |
|          | ------|       |  server  |
|----------|       |       |----------|
                   |
                   |       |----------|
                   |------>|          |
                           | 3rd party|
                           |    API   |
                           |----------|

```

Scheme B (my server making 3rd party HTTP request):
```

 /---------                |----------|
|          |  http calls   |          |
|  browser | ------------> |    my    |
|          |               |  server  |
|----------|               |----------|
                                |
                                |
                                \/
                           |----------|
                           |          |
                           | 3rd party|
                           |    API   |
                           |----------|

```


### Solution here please ...


Scheme A might be preferable due to decreased server load and the particular request; ie: if the call is very time sensitive.

If there is no need for credentialing or logging data it may even be ideal.