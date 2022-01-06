# CampusLine - a socializing and knowledge-sharing platform
A Social Nerworking Services(SNS) web application based on SpringBoot, Vue.js, Mybatis and Mysql


## Table of Contents
---
* [Introduction](introduction)
* [Technologies](technologies)
* [Functionalities](functionalities)
* [Structure](structure)
* [Launch](launch)
* [Examples](examples)

## Introduction
---
* CampusLine is a social networking & knowledge-sharing web application for students to address a couple of problems caused by online learning.

* It makes communicating with classmates about daily lives and course problems more convenient.

## Technologies
---
* For the whole system life cycle, we use agile development methods: Regular group meeting, GitLab version control, GitLab Issue Board and  Online sharing documents.

* For the front-end, we use Vue.js as the basic framework, and BootStrap to provide outlooks.

* For back-end, we use SpringBoot framework as fundemental framework.

* As for database, we choose Mybatis as persistence framework, Druid as connection pool, and Mysql as database.

* When testing our application, we use Junit for the unit testing, swagger-ui for interface testing and NightWatch for end-to-end testing.


## Functionalities
---
### Our application are generally used by 3 roles:
* Visitors: They can sign up, log in, browse homepage and hotposts, and search posts or users in the platform.

* Logined Users: They share the same functions visitors have. Besides, they can manage their profiles, publish posts, publish comments, like posts, follow their interested users, apply for module administrator, and send direct messages to others.

* Module Administrator: With the functions the above 2 roles have, they are given the authorization to create or delete modules, manage posts in their responsible modules.

## Sturcture
---
### This is  the main structure of back-end:
```
+---src
|   +---main
|   |   +---java
|   |   |   \---com
|   |   |       \---example
|   |   |           \---project
|   |   |               |   SpringBootProjectApplication.java
|   |   |               +---config
|   |   |               +---controller  
|   |   |               +---entity
|   |   |               +---mapper
|   |   |               +---result
|   |   |               +---service  
|   |   |               |   \---Impl 
|   |   |               \---utils
|   |   \---resources
|   |       |   application.yml
|   |       |   generatorConfig.properties
|   |       |   generatorConfig.xml
|   |       \---mapper
``` 
* SpringBootProjectApplication.java is the entrance of our application, the application will get started when runnning it.

* The folder controller comprises the interfaces between front-end and back-end.

* The foleder entity consists of entities in application.

* The folder mapper contains interfaces to manipulate database.

* The folder service contains service interfaces and their implementation.

* The folder utils contains utility classes needed by application.

* The folder resources contains configuration files and mybatis xml files.

### This is the main structure of front-end:
```
+---config
+---e2e_test       
+---mochawesome-report
+---node_modules
+---output    
+---reports       
+---src
|   |   App.vue
|   |   main.js
|   +---assets
|   +---components
|   +---router
|   +---test        
|   \---view
+---static                           
+---test      
\---tests_output
```


## Launch
---

## Examples