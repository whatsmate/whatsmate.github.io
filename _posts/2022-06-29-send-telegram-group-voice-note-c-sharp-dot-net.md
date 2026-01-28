---
layout: post
title: How to send a voice note file to a Telegram group in C# using Visual Studio 2019
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2026-01-28T20:11:00+08:00
---

This article shows you how to send a voice note file (e.g. an OPUS file) to a registered Telegram group in Microsoft's .NET language: C# using Visual Studio 2019.

If you are using Visual Studio 2022, please read [this tutorial](/2022-07-20-send-telegram-group-voice-note-c-sharp-dot-net-vs2022/) instead.

To send a Telegram message containing a voice note file in C# using Visual Studio 2019, do this:

1. First, learn how to send a simple text message to a group on the [official site](https://www.whatsmate.net/telegram-group-message-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/telegram-demos/archive/master.zip).
3. Locate the file `cs/group-send-telegram-opus.cs`.  <script src="https://gist.github.com/whatsmate/bdd23ecc3cf5ba52cf20b246ffa25ad4.js"></script>
4. Study the `C#` source code and customize the TODO/FIXME lines.
5. Run the `C#` program in Visual Studio to send your group your first OPUS file!


Happy coding :) 


<br>

