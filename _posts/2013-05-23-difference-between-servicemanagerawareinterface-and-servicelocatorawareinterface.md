---
layout: post
title: "Difference between ServiceManagerAwareInterface and ServiceLocatorAwareInterface"
description: ""
category: 
tags: [zf2, service manager]
---
{% include JB/setup %}

The `ServiceManagerAwareInterface` is a specific implementation of a service locator. It is currently considered deprecated, so should not be used.

Instead, you should use `\Zend\ServiceManager\ServiceLocatorAwareInterface` to make your classes service aware. And Zend also provides a  `\Zend\ServiceManager\ServiceLocatorAwareTrait` which you can use.

**More information:** 

- [http://zend-fr
amework-community.634137.n4.nabble.com/ServiceManagerAwareInterface-vs-ServiceLocatorAwareInterface-td4655675.html](http://zend-fr
amework-community.634137.n4.nabble.com/ServiceManagerAwareInterface-vs-ServiceLocatorAwareInterface-td4655675.html)
- [http://stackoverflow.com/questions/14930370/zend-framework-2-difference-between-servicemanagerawareinterface-and-servicelo](http://stackoverflow.com/questions/14930370/zend-framework-2-difference-between-servicemanagerawareinterface-and-servicelo)