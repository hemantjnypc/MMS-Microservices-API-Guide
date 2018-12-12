---
description: Processing RTU I/O data
---

# rtu.mms

|  | Description |
| :--- | :--- |
| rtu | relay, readCoil, humiture, air, ifr |
| rtutcp | relay, readCoil |

rtu@hello.ypcloud.com

| Function | Parameters | Return |
| :--- | :--- | :--- |
| **rtu\(\)** | {"name":"STRING","cmd":"STRING", "action":"STRING"} | {"RstCode":"STRING","RstMsg":"STRING","Data":"STRING"} |
| Relay controller | {"name":"yellowFan","cmd":"relay", "action":"open"} | {"RstCode":"0","RstMsg":"OK","Data":"Open success !!"} |
| **rtu\(\)** | {"name":"STRING","cmd":"STRING"} | {"RstCode":"STRING","RstMsg":"STRING","Data":"STRING"} |
| ReadCoil state | {"name":"yellowFan","cmd":"readCoil"} | {"RstCode":"0","RstMsg":"OK","Data":"Is open !!"} |
| **rtu\(\)** | {"name":"STRING","cmd":"STRING"} | {"RstCode":"STRING","RstMsg":"STRING","Data":"STRING"} |
| Get Humiture | {"name":"humitureSensor","cmd":"humiture"} | {"RstCode":"0","RstMsg":"OK","Data":"Temperature: 19.2˚C, Humidity: 48%RH"} |
| **rtu\(\)** | {"name":"STRING","cmd":"STRING"} | {"RstCode":"STRING","RstMsg":"STRING","Data":"STRING"} |
| Get Air | {"name":"airSensor","cmd":"air"} | {"RstCode":"0","RstMsg":"OK","Data":"PM2.5: 1ug/m3, PM10: 1ug/m3"} |
| **rtu\(\)** | {"name":"STRING","cmd":"STRING"} | {"RstCode":"STRING","RstMsg":"STRING","Data":"STRING"} |
| Get IFR | {"name":"ifrSensor","cmd":"ifr"} | {"RstCode":"0","RstMsg":"OK","Data":"Warning !!"} |
| **rtutcp\(\)** | {"name":"STRING","cmd":"STRING", "action":"STRING"} | {"RstCode":"STRING","RstMsg":"STRING","Data":"STRING"} |
| Relay controller | {"name":"redFan","cmd":"relay","action":"open"} | {"RstCode":"0","RstMsg":"OK","Data":"Open success !!"} |
| **rtutcp\(\)** | {"name":"STRING","cmd":"STRING"} | {"RstCode":"STRING","RstMsg":"STRING","Data":"STRING"} |
| ReadCoil state | {"name":"redFan","cmd":"readCoil"} | {"RstCode":"0","RstMsg":"OK","Data":"Is open !!"} |

