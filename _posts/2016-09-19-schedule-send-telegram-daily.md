---
layout: post
title: How to Send Yourself the Exchange Rate of a Currency Daily
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
---

This article shows you how to write a simple Python script to send yourself the exchange rate of Japanese YEN via the Telegram Gateway, and then schedule it to run daily.

Before the recipient can receive your Telegram message, she will need to register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](http://www.whatsmate.net/telegram-gateway-api.html). *Unregistered users will never receive messages from the Gateway.*


### Prerequisites:

1. You have access to a Linux (such as Ubuntu) machine.
2. Your machine has Python and the `requests` library installed.
3. You know some basic Python. Actually, it's alright even if you don't.



### Steps:

1. Take a look at this script: [exchange-rate-via-telegram.py](https://github.com/whatsmate/telegram-demos/blob/master/python/exchange-rate-via-telegram.py){:target="_blank"}. It retrieves the exchange rate of YEN and sends it to a target number you specify.
2. Customize the script to your liking. At least, specify your target number on line 50.
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



### Disclaimer:

1. The method described above aims to illustrate the concepts to send exchange rate information via Telegram only. We do not take any responsibilities for any financial gain/loss incurred due to your usage of the method.
2. The exchange rate information used in the script is provided by "fixer.io". We are NOT affiliated with "fixer.io" in any way. We are not responisble for the accuracy of the information either.
3. We are not affiliated with Telegram in any way. We only provide a gateway for sending out Telegram messages. We cannot guaranttee the gateway is functional at all times.

