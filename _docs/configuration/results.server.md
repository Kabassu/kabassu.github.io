---
title: io.kabassu.results.server.json
classes: wide
toc: false
---

```json
{
(...)
    "port": 8090,
    "resultsDir": "../../../reports-dir",
    "cerificatePath": "certificate/dev.p12",
    "password": "developer"
  }
}
```
- **port** - port where server will be available  
- **resultsDir** - directory where Kabassu downloads reports. This parameter has to be the same as **defaultReportsDir** in _io.kabassu.results.retriever.main.json_
- **cerificatePath** - certificate for ssl
- **password** - password for certificate