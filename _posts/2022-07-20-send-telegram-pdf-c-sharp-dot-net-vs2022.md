---
layout: post
title: How to send a PDF file to a Telegram user in C# using Visual Studio 2022
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2025-03-16T00:00:00+08:00
---

This article shows you how to send a document (e.g. a PDF file) to a registered Telegram user in Microsoft's .NET language: C# using Visual Studio 2022.

If you are using Visual Studio 2019, please read [this tutorial](/2022-06-20-send-telegram-pdf-c-sharp-dot-net/) instead.

Before the recipient can receive your Telegram message, she MUST register with the WhatsMate Telegram Gateway. Instructions are available on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). <span style="color:red">*Unregistered users will never receive messages from the Gateway.*</span>


<iframe width="560" height="315" src="https://www.youtube.com/embed/WkJmIC6Y4o8?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To send a Telegram message containing a PDF document in C# using Visual Studio 2022, do this:

1. First, learn how to send a simple text message on the [official site](https://www.whatsmate.net/telegram-gateway-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/telegram-demos/archive/master.zip).
3. Locate the file `cs_vs2022/send-telegram-pdf.cs`.  <script src="https://gist.github.com/whatsmate/24ec7c9123d11465593e77d9aad97f0d.js"></script>
4. Study the `C#` source code and customize the TODO/FIXME lines.
   * Among other things, put down YOUR OWN number as the recipient. You can't send messages to strangers because we are against SPAMMERS.
5. Run the `C#` program in Visual Studio to send yourself the first PDF file!


Happy coding :) 


<br>

