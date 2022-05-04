---
layout: post
title: How to Translate Text in Python
subtitle: Using the WhatsMate Translation REST API
published: true
last_modified_at: 2022-05-03T00:00:00+08:00
---

This article shows you how to translate text in Python.


<iframe width="560" height="315" src="https://www.youtube.com/embed/qeOQBpYSszA?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


To translate text (e.g. from English to Portuguese) from a Python script, do this:

1. Copy the following source code to your Python script.  <script src="https://gist.github.com/whatsmate/c0faa349997272fc74b18f2cbb8ece66.js"></script>
2. Specify the language code of the original text on line 10.
3. Specify the language code of your target language on line 11.
4. Specify the text that needs to be translated on line 12.
5. Install the `Requests` library because the sample script depends on it: `pip install requests`
6. Make your script executable: `chmod 755 translate-text.py`
7. Run the script to see the result: `./translate-text.py`


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

