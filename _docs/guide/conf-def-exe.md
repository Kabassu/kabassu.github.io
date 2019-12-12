---
title: Configurations, Definitions, Executions Guide
---

## General

Configurations, Definitions, Executions are three main data structures in Kabassu. 

**Definition** - it is template for the test. It contains required parameters to run it.

**Executions** - this is definition which was run or in other words instance of definition. It will contains reports, can be rerun with the same parameters etc. 

Both structures contains parameters that describe (like name or description) and _additional parameters_ which configure test we want to run.

Their dependency is quite simple. Definition has parameters and execution can override them. 

Example:
 
We have test prepared in definition and its location is in GIT and branch is master then we can just create execution that will run it.
But if we want to run the same test from branch develop we don't need to create new definition. We can create execution and override branch parameter.

**Configuration** - this is set of _additional parameters_ that can be reused in many definitions and executions. We can connect configuration to them and Kabassu will use parameters from configuration.
If there is the same parameter in configuration and definition then value from definition has priority. Same for configuration and execution.

## Example

**There are two configurations:**

*ConfigurationA* 
- parameter A: Text Value A
- parameter B: Text Value B

*ConfigurationB* 
- parameter C: Text Value C

**Definition was created and connected to ConfigurationA**

*DefinitionA*
- name: definition
- configuration: ConfigurationA

Additional Parameters:
- parameter B: Text Value Z

**Kabassu will merge ConfigurationA and Additional Parameters and result in the end**

*DefinitionA*
- name: definition

Additional Parameters:
- parameter A: Text Value A
- parameter B: Text Value Z

**Next step is create an execution from DefinitionA** 

*ExecutionA*
- name: execution
- configuration: ConfigurationB

**Kabassu will now merge all additional parameters and this will be execution to run**

*ExecutionA*
- name: execution   

Additional Parameters:
- parameter A: Text Value A
- parameter B: Text Value Z
- parameter C: Text Value C     
