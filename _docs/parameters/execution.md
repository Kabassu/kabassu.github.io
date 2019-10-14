---
title: Parameters - Execution
---

What parameters can be set in execution request:
- **description** - execution description
- **configurationId** - id of configuration with prepared additional parameters

Additional parameters (will override one from configuration):
 - **jvm** - used if gradle test required different _jvm_ then the one running Kabassu
 - **branch** - used with git and different branch then _master_
 - **domain** - used in AET - overrides domain from suite
 - **pattern** - used in AET - overrides patter from suite
 - **name** - used in AET - overrides name from suite
 
