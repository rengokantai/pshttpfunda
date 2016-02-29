#### pshttpfunda
#####1
###### encoding
legal chars:  
0-9 a-z A-Z $-_.+*'(),  

and memorize:
```
space %20
! %21
" %22
# %23
$ %24
% %25
& %26
```

#####2
######manual request
```
telnet google.com 80
```
then:
```
GET /a.jpg HTTP/1.1
Host: www.google.com
```
######Request message
common request headers
```
Connection: keep-alive
Referer
User-Agent
Accept
Accept-Language
Cookie
If-Modified-Since //date of last retrival
Date //creation timestamp of message
```
q value: relative degree. default=1.0. Ex
```
utf-8;q=0.7,*;q=0.3    //utf-8 70% like else 30% like
```
#####3
######whirl network
application->http  transport-TCP network->ip datalink->ethernet  
######Peristent conn
typically, shared server website we can see
```
Connection:close
```
in response header. If server is standup,it will not show
