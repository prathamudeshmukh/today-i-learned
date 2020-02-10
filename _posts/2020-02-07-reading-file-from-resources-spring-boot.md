---
layout: post
title: "Reading file from resources folder in Spring Boot"
description: "How would you read a file from resources folder?"
tags: [spring-boot, java, file]
---
You should be using `getResourceAsStream(...);`
when the resource is bundled as a JAR/WAR or any other single file package for that matter.
A JAR is a single file (kind of like a zip file) holding lots of files together. From OS's point of view, its a single file and if you want to access a part of the file you must use it as a stream.

This applies to the json,txt,csv files you may have added to the `resources` folder of your spring boot project structure.
Your code will work if you are running in an IDE, since IDE does not generate a jar file, but when running from CLI, the program will not be able to find the file, since it is in a JAR.