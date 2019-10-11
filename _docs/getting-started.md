---
title: Getting started - Kabassu
---

## Description
The goal of Kabassu is to create test central, place where users can gather different tests for different application, run them against different enviroments and configurations

## Requirements

1. Java 12
2. MongoDB
3. Allure 2.7.0 added to path (if allure-trend reports are used)

## How to run it

1. Go through [installation](/docs/installation) and [configuration](/docs/configuration/configuration) processes. 
2. Run start.bat or start.sh
3. Application will use ports 8080 and 8090. These ports can be changed in server configuration files

## API

Kabassu is run by calling series of rest services. All available endpoints can be found in [OpenApi specification](https://github.com/Kabassu/kabassu/tree/master/configuration/openapi/kabassu_api.yaml) in OpenApi 3 format that can be opened using Swagger Editor   

## Guides

- [Guide for single test](/docs/guide/singletest) 
- [Guide for test suit](/docs/guide/testsuite)   
- [Guide for AET test](/docs/guide/aettest)

## GUI

We recommend using our GUI which is easier then calling API. You can find starting guide [here](/docs-gui/getting-started) 