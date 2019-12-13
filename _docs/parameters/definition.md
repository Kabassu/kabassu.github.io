---
title: Parameters - Definition
---

What parameters can be set in definition request:
- **name** - definition name
- **runner** - what runner is used for the test
- **locationType** - where are test kept
- **configurationId** - id of configuration with prepared additional parameters

Additional parameters (will override one from configuration):
 - **runnerOptions** - used for runners that require additional parameters (for example _clean test_ for gradle)
 - **repository** - address of git repository (if git was chosen as test location type)
 - **location** - test location on disk (if filesystem was chosen as test location type)
 - **reportDir** - reports location for generic reports retrieve
 - **startHtml** - starting file for reports for generic reports retrieve
 - **server** - server address for AET tests 
 - **port** - port for AET tests
 - **suite** - suite for AET Tests
 - **jvm** - used if gradle test required different _jvm_ then the one running Kabassu
 - **branch** - used with git and different branch then _master_
 - **domain** - used in AET - overrides domain from suite
 - **pattern** - used in AET - overrides patter from suite
 - **name** - used in AET - overrides name from suite
 - every Lighthouse command line parameter can be added here
 
 
