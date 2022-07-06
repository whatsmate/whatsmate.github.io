---
layout: post
title: How to send an audio file to a Telegram group from bash shell script
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2022-06-28T00:00:00+08:00
---

This article shows you how to send an audio file (e.g. an MP3 file) to a registered Telegram group from a bash shell script.



To send a Telegram message containing an audio file to a group from a bash shell script, do this:

1. First, learn how to send a simple text message to a group on the [official site](https://www.whatsmate.net/telegram-group-message-api.html).
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/telegram-demos/archive/master.zip).
3. Locate the file `bash/group-send-telegram-mp3.sh`.  <script src="https://gist.github.com/whatsmate/e204b7e3597418d80ae376c8bbfd6a82.js"></script>
4. Study the script and customize the TODO/FIXME lines.
5. Change to the directory containing the script: `cd bash`
6. Run the script to send your group the first MP3 file: `./group-send-telegram-mp3.sh`


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

