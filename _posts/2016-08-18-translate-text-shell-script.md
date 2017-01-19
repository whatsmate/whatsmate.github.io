---
layout: post
title: How to Translate Text from shell script
subtitle: Using the WhatsMate Translation REST API
published: true
---

This article shows you how to translate text from a shell script.

To translate text (e.g. from English to Indonesian) from a shell script, do this:

1. Copy the following source code to your script.  <script src="https://gist.github.com/whatsmate/0199d2796aadff6ff8631163c1b3efcd.js"></script>
2. Specify the language code of the original text on line 8.
3. Specify the language code of your target language on line 9.
4. Specify the text that needs to be translated on line 10.
5. Make your script executable: `chmod 755 translate-text.sh`
6. Run the script to see the result: `./translate-text.sh`


Looking for your language code? See the <a target="_blank" href="http://api.whatsmate.net/v1/translation/supported-codes">complete listing</a>.


The trial account only allows you to call the translation API up to 10 times for learning purpose. [Subscribe to a Premium plan](https://www.whatsmate.net/translation-subscribe.html) to use the translation API seriously.


Want to translate text in another programming language? Check out the [Translation API](https://www.whatsmate.net/translation-api.html) page.


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

