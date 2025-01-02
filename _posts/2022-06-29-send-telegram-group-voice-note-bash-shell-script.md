---
layout: post
title: How to send a voice note file to a Telegram group from bash shell script
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2025-01-02T00:00:00+08:00
---

This article shows you how to send a voice note file (e.g. an OPUS file) to a registered Telegram group from a bash shell script.



To send a Telegram message containing a voice note file to a group from a bash shell script, do this:

1. First, learn how to send a simple text message to a group on the [official site](https://www.whatsmate.net/telegram-group-message-api.html).
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/telegram-demos/archive/master.zip).
3. Locate the file `bash/group-send-telegram-opus.sh`.  <script src="https://gist.github.com/whatsmate/514f055417f5724f1c2de37eadc975cf.js"></script>
4. Study the script and customize the TODO/FIXME lines.
5. Change to the directory containing the script: `cd bash`
6. Run the script to send your group the first OPUS file: `./group-send-telegram-opus.sh`


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

