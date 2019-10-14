---
title: Troubleshooting
---

Solutions for some problems that users can found:

```
**PROBLEM**    
Can't login with correct credentials.

**ANSWER**   
Two possible solutions:
- check if you have latest browser version
- try to call https://<your_address>/kabassu/login directly and add certificate to trusted
```

```
**PROBLEM**    
Options added to backend configuration are not available in dropdowns

**ANSWER**   
Go to components/data/data.js - add entry to correct type:
  - jvmValues - for jvms
  - suggestedTypes - configuration types
  - locationTypes - where tests are kept
  - runnerTypes - runner for tests
  - reportTypes - new reports
``` 



