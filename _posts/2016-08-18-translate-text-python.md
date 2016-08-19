---
layout: post
title: How to Translate Text in Python
subtitle: Using the WhatsMate Translation REST API
published: true
---

This article shows you how to translate text in Python.

To translate text (e.g. from English to Spanish) from a Python script, do this:

1. Copy the following source code to your Python script.  <script src="https://gist.github.com/whatsmate/c0faa349997272fc74b18f2cbb8ece66.js"></script>
2. Specify the language code of the original text on line 10.
3. Specify the language code of your target language on line 11.
4. Specify the text that needs to be translated on line 12.
5. Make your script executable: `chmod 755 translate-text.py`
6. Run the script to see the result: `./translate-text.py`


Looking for your language code? See the <a target="_blank" href="http://api.whatsmate.net/v1/translation/supported-codes">complete listing</a>.


The trial account only allows you to call the translation API up to 10 times for learning purpose. [Subscribe to a Premium plan](http://www.whatsmate.net/translation-subscribe.html) to use the translation API seriously.


Want to translate text in another programming language? Check out the [Translation API](http://www.whatsmate.net/translation-api.html) page.

