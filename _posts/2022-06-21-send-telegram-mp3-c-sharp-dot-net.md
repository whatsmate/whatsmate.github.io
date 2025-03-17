---
layout: post
title: How to send an audio file to a Telegram user in C# using Visual Studio 2019
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2025-03-16T00:00:00+08:00
---

This article shows you how to send an audio file (e.g. an MP3 file) to a registered Telegram user in Microsoft's .NET language: C# using Visual Studio 2019.

If you are using Visual Studio 2022, please read [this tutorial](/2022-07-20-send-telegram-mp3-c-sharp-dot-net-vs2022/) instead.

To send a Telegram message containing an audio file in C# using Visual Studio 2019, do this:

1. First, learn how to send a simple text message on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/telegram-demos/archive/master.zip).
3. Locate the file `cs/send-telegram-mp3.cs`.  <script src="https://gist.github.com/whatsmate/c7ad4f16fc683d1bec2ed86c839b9fac.js"></script>
4. Study the `C#` source code and customize the TODO/FIXME lines.
   * Among other things, put down YOUR OWN number as the recipient. You can't send messages to strangers because we are against SPAMMERS.
5. Run the `C#` program in Visual Studio to send yourself the first MP3 file!


Happy coding :) 


<br>

