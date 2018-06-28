---
layout: post
title:      "Class vs. Instance Method "
date:       2018-06-28 19:27:34 +0000
permalink:  class_vs_instance_method
---


When a class method is identified outside of physical code, it is preceded with a period, such as '.all'. An instance method, on the other hand, is preceded by a hashtag, such as '#save'. 

To understand the difference between the two and determine when to use each, consider what the method is acting upon. 

For instance, above I used the examples ‘.all’ and ‘#save’. These methods are typically seen in these varieties. The #save method acts on each instance of a class, therefore it is an instance method. The .all method displays every instance of the class, therefore it is a class method -- it has no effect on any single instance. 

