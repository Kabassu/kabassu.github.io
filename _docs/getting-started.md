---
title: Getting started - Kabassu
---

This manual is for [lastest released version](https://github.com/Kabassu/kabassu/releases/latest)

## Description
The goal of Kabassu is to create test central, place where users can gather different tests for different application, run them against different enviroments and configurations

## Requirements

1. Java 12
2. MongoDB
3. Allure 2.7.0 added to path (if allure-trend reports are used)

## How to run it

1. Create database in Mongo.
2. Clone this repository
3. Build with gradle
4. Go to distribution folder, unzip zip file in desired location
5. Go to configuration/modules/io.kabassu.mongo.json and change entry:
 ```
  "mongo-config": {
       "db_name": "kabassu-dev"
 ```
Here you can find possible options [https://vertx.io/docs/vertx-mongo-client/java/#_configuring_the_client]

6. Run start.bat or start.sh
7. Application will use ports 8080 and 8090. They can be changed in server configuration files

More detailed information can be found:  
[Installation](/docs/installation)  
[Configuration](/docs/configuration/configuration)

## API

Kabassu is run by calling series of rest services. All available endpoints can be found in OpenApi specification _configuration/openapi_   
[Guide for single test](/docs/guide/singletest) and [Guide for test suit](/docs/guide/testsuite) explain using of API  

Every endpoint can be found [here](configuration/openapi/kabassu_api.yaml) in OpenApi 3 format that can be opened using Swagger Editor
