---
layout: post
title: How to Send Yourself a Stock Price Alert via Telegram
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
---

<img src="/img/chart-small-hd.png" height="100" width="100" />

This article shows you how to write a simple Python script to monitor your beloved stock and send an alert to yourself when it hits your target price. Read on to get rich from your capital gain :)


<p style="text-align:center;">
  <img src="/img/stock-telegram.jpg"/>
</p>


Before you can receive the Telegram message, you will need to register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). *Unregistered users will never receive messages from the Gateway.*


### Prerequisites:

1. You have access to a Linux (such as Ubuntu) machine.
2. Your machine has Python and the `requests` library installed.
3. You know some basic Python. Actually, it's alright even if you don't because our code looks like simple English.
4. You know how to set up a cron job. Actually, it's alright even if you don't because we will tell you how.


### Steps:

1. Take a look at this script: [stock-price-alert-via-telegram.py](https://github.com/whatsmate/telegram-demos/blob/master/python/stock-price-alert-via-telegram.py){:target="_blank"}. It gets a price quote of your stock, checks to see if it has hit your target price and sends a Telegram alert to you only when the price is good.
2. Customize the script to your liking. At least, specify your target number on line 55.
3. Take note of the location of your script. For example: `/home/pikachu/stock-price-alert-via-telegram.py`
4. Give the execute permission to your script: `chmod 755 /home/pikachu/stock-price-alert-via-telegram.py`
5. Run the script once to confirm if it really works.
6. Schedule the script to run at - say - 2pm on Monday through Friday: 
   1. On the command prompt, type this: `crontab -e`
   2. It will then open an editor (e.g. vi) for you to edit the content of your crontab entries.
   3. Add a line like this one:  
      `00 14 * * 1-5   /home/pikachu/stock-price-alert-via-telegram.py`
   4. Save the changes and exit the editor.
7. You're done. Now you just need to wait for your stock to hit your target price :)


### Explanation:

If you are new to Python and want to understand how the Python script works, we are here to help:

1. In lines 6 through 15, the function `getStockQuote()` is defined. It obtains a price quote from Yahoo Finance and returns it.  Check out [this article](https://kx.cloudingenium.com/content-providers/how-to-obtain-stock-quotes-from-yahoo-finance-you-can-query-them-via-excel-too/){:target="_blank"} if you want to learn more about how Yahoo Finance works.
2. In lines 18 through 41, the function `sendTelegramMessage()` is defined. It sends a Telegram message to a designated number via our Telegram Gateway.
3. In lines 44 through 62, the function `main()` is defined. It calls `getStockQuote()` to get a price quote of the the Apple stock. Then it checks to see if it's higher than $120. If so, it calls `sendTelegramMessage()` to send out an alert message.


<br>
<script async src="//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
<ins class="adsbygoogle"
     style="display:inline-block;width:728px;height:90px"
     data-ad-client="ca-pub-7383487179928477"
     data-ad-slot="6959057004"></ins>
<script>
(adsbygoogle = window.adsbygoogle || []).push({});
</script>
<br>


### Disclaimer:

1. The method described above aims to illustrate the concepts to send a stock price alert via Telegram only. We do not take any responsibilities for any financial gain/loss incurred due to your usage of the method.
2. The stock price quote used in the script is provided by Yahoo Finance. We are NOT affiliated with Yahoo Finance in any way. We are not responisble for the accuracy of the price quotes either.
3. We are not affiliated with Telegram in any way. We only provide a gateway for sending out Telegram messages. We cannot guaranttee the gateway is functional at all times.

