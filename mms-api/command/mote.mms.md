---
description: MoteBus integration
---

# mote.mms

|  | Description |
| :--- | :--- |
| Add | Add numbers |
| Echo | Send back the same message |
| Time | To know what time it is |

mote@hello.ypcloud.com

| Function | Parameters | Return |
| :--- | :--- | :--- |
| **Add\(\)** | {"A":"INT","B":"INT"} | {"C":"INT"} |
|  | {"A":"28","B":"37"} | {"C":"65"} |
| **Echo\(\)** | {"Data":"STRING"} | {"Result":"STRING"} |
|  | {"Data":"HelloWorld" } | {"Result":"HelloWorld"} |
| **Time\(\)** | {"Data":"STRING"} | {"Result":"STRING"} |
|  | {"Data":""} | {"Result":"2018-03-13T03:43:30.185Z"} |

