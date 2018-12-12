---
description: Get & manage the VM (compute & storage) states
---

# gcp.mms

|  | Description |
| :--- | :--- |
| on | turn on a VM instance |
| off | turn off a VM instance |
| status | status of VM instance\(s\) |
| create | create a VM instance |
| delete | delete a VM instance |

gcp@hello.ypcloud.com

| Function | Parameters | Return |
| :--- | :--- | :--- |
| **vm\(on\)** | {"cmd":"on", "name":"STRING"} | {"OpType":"STRING","Status":"STRING", "InsertTime":"STRING"} |
|  | {"cmd":"on","name":"instance\_test\_01"} | {"OpType":"start","Status":"PENDING","InsertTime":"2018-01-31T00:08:11.629-08:00"} |
| **vm\(off\)** | {"cmd":"off", "name":"STRING"} | {"OpType":"STRING","Status":"STRING", "InsertTime":"STRING"} |
|  | {"cmd":"off","name":"instance\_test\_01"} | {"OpType":"stop","Status":"PENDING","InsertTime":"2018-01-31T00:08:11.629-08:00"} |
| **vm\(Status\)** | {"cmd":"status", "name":"STRING", "os":"STRING"} | {"name":"STRING", "zone":"STRING", "status":"STRING"} |
|  | {"cmd":"status", "name":"instance-1xyzabc"} | {"name":"instance-1xyzabc", "zone":"asia-east1-a", "status":"TERMINATED"} |
| **vm\(create\)** | {"cmd":"create", "name":"STRING", "os":"STRING"} | {"VmName":"STRING", "OpType":"STRING", "Status":"STRING", "InsertTime":"STRING"} |
|  | {"cmd":"create", "name":"instance-1xyzabc"} | {"VmName":"STRING","OpType":"insert","Status":"RUNNING","InsertTime":"2018-01-31T00:08:11.629-08:00"} |
| **vm\(delete\)** | {"cmd":"delete", "name":"STRING"} | {"VmName":"STRING","OpType":"STRING","Status":"STRING","InsertTime":"STRING"} |
|  | {"cmd":"delete", "name":"instance-1xyzabc"} | {"VmName":"instance-1xyzabc","OpType":"delete","Status":"PENDING","InsertTime":"2018-01-31T00:08:11.629-08:00"} |

