---
layout: post
title: How to send a PDF file to a WhatsApp group in C# (.NET) using Visual Studio 2019
subtitle: Using the WhatsMate WhatsApp Gateway REST API
published: true
last_modified_at: 2025-03-16T00:00:00+08:00
---

This article shows you how to send a document (e.g. a PDF file, an MP4 file, a WAV file, etc.) document to a WhatsApp group in Microsoft's .NET language: C# using Visual Studio 2019.

If you are using Visual Studio 2022, please read [this tutorial](/2022-07-18-send-whatsapp-pdf-group-c-sharp-dot-net-vs2022/) instead.

To send a PDF document to a WhatsApp group in C#, do this:

1. First, learn how to send a simple text message to a group on the [official site](https://www.whatsmate.net/whatsapp-group-message-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/wa-demos/archive/master.zip).
3. Locate the file `cs/send-pdf-group.cs`.  <script src="https://gist.github.com/whatsmate/9bb8f3301054d7c739a011303f9513c5.js"></script>
4. Study the `C#` source code and customize the TODO/FIXME lines.
   * Among other things, you must name your group *creatively*. Otherwise, the group may not receive the message.
5. Run the `C#` program in Visual Studio to send your group the first PDF file!


Happy coding :) 


<br>

