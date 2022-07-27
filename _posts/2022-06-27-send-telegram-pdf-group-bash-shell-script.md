---
layout: post
title: How to send a PDF file to a Telegram group from shell script
subtitle: Using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2022-06-27T00:00:00+08:00
---

This article shows you how to send a document (e.g. a PDF file etc.) to a registered Telegram group from a shell script.

<iframe width="560" height="315" src="https://www.youtube.com/embed/5O3ZpZ1CfzI?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>

To send a PDF document to a Telegram group from a shell script, do this:

1. First, learn how to send a simple text message to a group on the [official site](https://www.whatsmate.net/telegram-group-message-api.html).
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/telegram-demos/archive/master.zip).
3. Locate the file `bash/group-send-telegram-pdf.sh`.  <script src="https://gist.github.com/whatsmate/3d863e5beca363d71ecf205401dd5322.js"></script>
4. Study the script and customize the TODO/FIXME lines.
5. Change to the directory containing the script: `cd bash`
6. Run the script to send the group the first PDF: `./group-send-telegram-pdf.sh`

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

