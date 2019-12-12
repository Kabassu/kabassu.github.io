---
title: Views
---

Views are way to group different test executions together. For example all test for one enviroment or all performance tests. Execution can be in many views.

It is also possible to run all tests grouped in view.

## Create view

To create view POST call should be made to _/kabassu/addview/_

Required POST parameters:

- **name** - view name
- **description** - view description          
- **executionId** - array of executions id

## Add or remove execution from existing view

This is POST call to _/kabassu/updateview/_

Required POST parameters:

- **id** - view id           
- **field** - should be always _executionId_          
- **value** - execution id          
- **operation** -  _add_ or _remove__

## Run all executions in view

This is POST call to _/kabassu/view/run/_

Required POST parameters:

- **viewId** - view id             
        

