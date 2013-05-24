---
layout: post
title: "Trigger cron job in Magento"
description: ""
category: 
tags: [magento, cron job]
---
{% include JB/setup %}

Often when you're developing or debugging a cron job in Magento, you want a quick way to trigger the cron job without having to schedule it each time or wait for it to start running.

In the root of your project, create a file `runcronjob.php` with the following code:

    <?php
    	require 'app/Mage.php';
    	Mage::init('admin');
    	Mage::getModel('my_module/observer')->runMyCronJob();

Then load the file in your browser:

    http://localhost/runcronjob.php

Or alternatively, you can also run it from command line: 

    $ php /var/www/src/runcronjob.php

This is especially useful when your script times out.