---
layout: post
title: How to send a PDF file to a WhatsApp group from shell script
subtitle: Using the WhatsMate WhatsApp Gateway REST API
published: true
last_modified_at: 2019-12-06T00:00:00+08:00
---

This article shows you how to send a document (e.g. a PDF file, an MP4 file, a WAV file, etc.) to a registered WhatsApp group from a shell script.


To send a PDF document to a WhatsApp group from a shell script, do this:

1. First, learn how to send a simple text message to a group on the [official site](https://www.whatsmate.net/whatsapp-group-message-api.html).
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/wa-demos/archive/master.zip).
3. Locate the file `bash/send-pdf-group.sh`.  <script src="https://gist.github.com/whatsmate/d58030fa593d0f7893a5807a056a310a.js"></script>
4. Study the script and customize the TODO/FIXME lines.
   * Among other things, you must name your group *creatively*. Otherwise, the group may not receive the message.
5. Change to the directory containing the script: `cd bash`
6. Run the script to send the group the first PDF: `./send-pdf-group.sh`

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

