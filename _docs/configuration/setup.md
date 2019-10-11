---
title: io.kabassu.setup.json
classes: wide
toc: false
---

```json
{
  "name": "standard:io.kabassu.setup",
  "config": {
    "verticle": "io.kabassu.setup.KabassuSetupVerticle",
    "users": [
      {
        "username": "admin",
        "password": "admin"
      }
    ]
  }
}
```
**users** array of default users that should be created in database. - For security reasons entries should be deleted after first run

