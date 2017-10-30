---
layout: post
title: How to send an image to a WhatsApp group from shell script
subtitle: Using the WhatsMate WhatsApp Gateway REST API
published: true
last_modified_at: 2017-10-26T00:00:00+08:00
---

This article shows you how to send an image to a WhatsApp group from a shell script.


To send an image to a WhatsApp group from a shell script, do this:

1. First, learn how to send a simple text message to a group on the [official site](https://www.whatsmate.net/whatsapp-group-message-api.html). 
2. With the above knowledge, you can now download our [sample code](https://github.com/whatsmate/wa-demos/archive/master.zip).
3. Locate the file `bash/send-image-group.sh`.  <script src="https://gist.github.com/whatsmate/3392b82db3187565d19097bd5c22bfd2.js"></script>
4. Study the script and customize the TODO/FIXME lines.
   * Among other things, you must name your group *creatively*. Otherwise, the group may not receive the message.
5. Change to the directory containing the script: `cd bash`
6. Run the script to send the group the first image: `./send-image-group.sh`


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

