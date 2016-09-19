---
layout: post
title: How to Send Yourself the Exchange Rate of a Currency Daily
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
---

This article shows you how to write a simple Python script to send yourself the exchange rate of Japanese YEN via the Telegram Gateway, and then schedule it to run daily.

Before the recipient can receive your Telegram message, she will need to register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](http://www.whatsmate.net/telegram-gateway-api.html). *Unregistered users will never receive messages from the Gateway.*

Prerequisites:

1. You have access to a Linux (such as Ubuntu) machine.
2. Your machine has Python and the `requests` library installed.
3. You know some basic Python. Actualy, it's alright even if you don't.



Steps:

1. Take a look at this script: [send-telegram-exchange-rate.py](https://github.com/whatsmate/telegram-demos/blob/master/python/send-telegram-exchange-rate.py). It retrieves the exchange rate of YEN and sends it to a target number you specify.
2. Customize the script to your liking. At least, specify your target number on line 31.
3. Take note of the location of your script. For example: `/home/pikachu/send-telegram-exchange-rate.py`
4. Give the execute permission to the script: `chmod 755 /home/pikachu/send-telegram-exchange-rate.py`
5. Run the script once to confirm if it really works.
6. Schedule the script to run daily at 9am: 
   1. On the command prompt, type this: `crontab -e`
   2. It will then open an editor (e.g. vi) for you to edit the content of your crontab entries.
   3. Add a line like this one:  
      `00 09 * * *    /home/pikachu/send-telegram-exchange-rate.py`
   4. Save the changes and exit the editor.
7. You're done. You will receive the exchange rate every day.

