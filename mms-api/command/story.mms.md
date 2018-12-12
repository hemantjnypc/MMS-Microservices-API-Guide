---
description: Search for keyword(s) across DDNs and target_devices
---

# story.mms

|  | Description |
| :--- | :--- |
| search | To search a string keyword within an App to the &lt;DDN-&gt;target&gt; levels |

story@hello.ypcloud.com

| Function | Parameters | Return |
| :--- | :--- | :--- |
| **search\(\)** | {"app":"STRING","keyword":"STRING","ddn":\["STRING"\],"target":\["STRING"\]} | {"result":"STRING"} |
|  | {"app":"jujue","keyword":"mayday","ddn":\["ddn1","ddn2" \],"target":\["ylobby","ystand" \]} | {"result":"OK"} |

