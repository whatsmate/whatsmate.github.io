---
layout: post
title: How to Send Yourself Weather Info of a City via Telegram
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2017-03-31T00:00:00+08:00
---

<img src="/img/sun-cloud2.png"/>

This article shows you how to write a simple Python script to retrieve the weather condition of a city from Yahoo APIs and send it to yourself.


<p style="text-align:center;">
  <img src="/img/weather-telegram.jpg"/>
</p>


Before you can receive the Telegram message, you will need to register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


### Prerequisites:

1. You have access to a Linux (such as Ubuntu) machine.
2. Your machine has Python and the `requests` library installed.
3. You know some basic Python. Actually, it's alright even if you don't because our code looks like simple English.
4. You know how to set up a cron job. Actually, it's alright even if you don't because we will tell you how.


### Steps:

1. Take a look at this script: [weather-reminder-via-telegram.py](https://github.com/whatsmate/telegram-demos/blob/master/python/weather-reminder-via-telegram.py){:target="_blank"}. It gets the current weather information of Mountain View in California and sends it to a designated Telegram number.
2. Customize the script to your liking. At least, specify your target number on line 52.
3. Take note of the location of your script. For example: `/home/pikachu/weather-reminder-via-telegram.py`
4. Give the execute permission to your script: `chmod 755 /home/pikachu/weather-reminder-via-telegram.py`
5. Run the script once to confirm if it really works.
6. Schedule the script to run at - say - 10am daily: 
   1. On the command prompt, type this: `crontab -e`
   2. It will then open an editor (e.g. vi) for you to edit the content of your crontab entries.
   3. Add a line like this one:  
      `00 10 * * *  /home/pikachu/weather-reminder-via-telegram.py`
   4. Save the changes and exit the editor.
7. You're done. You will receive an update on the weather condition of Mountain View every day:)


### Explanation:

If you are new to Python and want to understand how the Python script works, we are here to help:

1. In lines 6 through 17, the function `getWeatherCondition()` is defined. It obtains the weather information of the specified city. Check out [Yahoo's official page](https://developer.yahoo.com/weather/){:target="_blank"} to learn more about how Yahoo APIs work.
2. In lines 20 through 43, the function `sendTelegramMessage()` is defined. It sends a Telegram message to a designated number via our Telegram Gateway.
3. In lines 46 through 59, the function `main()` is defined. First, it calls `getWeatherCondition()` to get the weather informaton of Mountain View. Then, it calls `sendTelegramMessage()` to send out the info.


### Disclaimer:

1. The weather information is provided by Yahoo APIs. We are NOT affiliated with Yahoo APIs in any way. We are not responisble for the accuracy of the data either.
2. We are not affiliated with Telegram in any way. We only provide a gateway for sending out Telegram messages. We cannot guaranttee the gateway is functional at all times.


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
