---
layout: post
title: How to send an image to a Telegram user in C# using Visual Studio 2019
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2025-01-02T00:00:00+08:00
---

This article shows you how to send an image to a registered Telegram user in Microsoft's .NET language: C# using Visual Studio 2019.

If you are using Visual Studio 2022, please read [this tutorial](/2022-07-20-send-telegram-image-c-sharp-dot-net-vs2022/) instead.

Before the recipient can receive your Telegram message, she MUST register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


To send a Telegram message containing an image in C# using Visual Studio 2019, do this:

1. First, learn how to send a simple text message on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/telegram-demos/archive/master.zip).
3. Locate the file `cs/send-telegram-image.cs`.  <script src="https://gist.github.com/whatsmate/ace3b9000bf160ef000fbf0c6b92c9eb.js"></script>
4. Study the `C#` source code and customize the TODO/FIXME lines.
   * Among other things, put down YOUR OWN number as the recipient. You can't send messages to strangers because we are against SPAMMERS.
5. Run the `C#` program in Visual Studio to send yourself the first image!


Happy coding :) 


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

