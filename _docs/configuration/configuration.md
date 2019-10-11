---
title: Configuration
classes: wide
toc: false
---

Configuration involves changing files placed in _configuration/modules_ directory in your Kabassu installation.
Not every file has to be changed, in fact if file is not described here the the best approach is to not touch it. Uncontrolled changes can break Kabassu  

**Also please change only described parameters and make sure that configuration file is still valid json file after these changes**

1. [io.kabassu.setup.json](../setup) - setup configuration. Used for setting start parameters in database. Usually deleted after first start.
1. [io.kabassu.server.json](../server) - server configuration. We suggest changing certificate and secret fo JWT  
2. [io.kabassu.runner.gradle.json](../runner.gradle) - runner responsible for running all test that use _gradle_ here JVM are set  
**Need to be changed before start**   
3. [io.kabassu.results.retriever.main.json](../retriever.main) - configuration for retrieving reports.
4. [io.kabassu.mongo.json](../mongo) - configuration of Mongo connection  
**Need to be changed before start**   
5.[io.kabassu.results.server.json](../results.server) - configuration of server that will provide access to download reports in html format. We suggest changing certificate   
**Has to be changed if directory in _io.kabassu.results.retriever.main.json_ was changed**
6. [io.kabassu.files.retriever.json](../files.retriever) - configuration for getting test files from other places then local filesystem
