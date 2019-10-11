---
title: How to install Kabassu
---

## Requirements

1. Java 12 - it is required to run Kabassu and should be main jvm installed in system
2. Any other JVM required to run tests. The JVMs shouldn't be in PATH (this is the place for 12) but there should be on disk
3. MongoDB
4. Allure 2.7.0 added to path (if allure-trend reports are used). Higher versions should work but are not supported for now
5. Git - if you want to download test using it. As for now only ssh access (key without password) is supported
6. AET server - if you want to run AET tests
7. Kabassu-GUI - it is not required but we recommand it as easiest way for using Kabassu Rest Services. It can be found [here](https://github.com/Kabassu/kabassu-gui) 

## Installation process

1. Install all positions from the requirements list
2. Run MongoDB and create an empty database
3. Download latest release (or checkout this repository - we suggest master branch as the most stable)
4. If using repository: build project using ```gradlew``` and take zip from _distribution_ folder
5. Uzip distribution in desired location
6. Configure Kabassu using guidelines from [here](/docs/configuration/configuration)
7. Run Kabassu using ```start.bat or start.sh```
