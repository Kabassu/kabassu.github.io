---
title: Login Guide
---

Endpoint: ``POST /kabassu/login``

Request:
```json
{
  "username":	"<login>",
  "password_hash": "<password_not_hashed>"  
}
```

- **username** - login for the account 
- **password_hash** - password - it shouldn't be hashed

Accounts are created at first run (or added directly to database). Please check [here](/docs/configuration/setup)

In response there will be access token that need to be used with other calls

```json
{
 "auth_token": "<access_token>"
}
``` 