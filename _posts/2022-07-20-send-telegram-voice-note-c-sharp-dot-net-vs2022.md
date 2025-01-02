---
layout: post
title: How to send a voice note file to a Telegram user in C# using Visual Studio 2022
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2025-01-02T00:00:00+08:00
---

This article shows you how to send a voice note file (e.g. an OPUS file) to a registered Telegram user in Microsoft's .NET language: C# using Visual Studio 2022.

If you are using Visual Studio 2019, please read [this tutorial](/2022-06-22-send-telegram-voice-note-c-sharp-dot-net/) instead.

Before the recipient can receive your Telegram message, she MUST register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


To send a Telegram message containing a voice note file in C# using Visual Studio 2022, do this:

1. First, learn how to send a simple text message on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/telegram-demos/archive/master.zip).
3. Locate the file `cs_vs2022/send-telegram-opus.cs`.  <script src="https://gist.github.com/whatsmate/d472c3e5df3b4757b0064e352ea942de.js"></script>
4. Study the `C#` source code and customize the TODO/FIXME lines.
   * Among other things, put down YOUR OWN number as the recipient. You can't send messages to strangers because we are against SPAMMERS.
5. Run the `C#` program in Visual Studio to send yourself the first voice note!


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

