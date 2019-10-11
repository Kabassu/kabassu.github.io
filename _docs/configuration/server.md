---
title: io.kabassu.server.json
classes: wide
toc: false
---

```json
{
  "name": "standard:io.kabassu.server",  
  "config": {  
(...)      
    "port": 8080,
    "security": "jwt",
    "cerificatePath": "certificate/dev.p12",
    "password": "developer",
    "jwtSecret": "jwt_secret_change_me",   
 (...)  
}
```
- **port** - select port where Kabassu Rest Services will be available 
- **cerificatePath** - certificate for ssl
- **password** - password for certificate
- **jwtSecret** - secret used for access token creation. Please change it