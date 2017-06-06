---
layout: post
title: How to Convert a PDF file to text in Python
subtitle: Using the WhatsMate PDF-to-Text REST API
published: true
last_modified_at: 2017-06-07T00:00:00+08:00
---

This article shows you how to extract text from an online PDF document in Python.


Here's how:

1. Copy the following source code to your Python script.  <script src="https://gist.github.com/whatsmate/40fceaea9ca177852b1488eaaeefc870.js"></script>
2. Specify the URL of your online PDF document on line 10.
3. Replace the Client ID and Secret on lines 5 and 6 if you have your own credentials.
5. Install the `Requests` library because the sample script depends on it: `pip install requests`
6. Make your script executable: `chmod 755 extract-pdf-text-sync.py`
7. Run the script to see the result: `./extract-pdf-text-sync.py`


If your PDF file is larger than 1 MB, you will need to call the asynchronous API instead.


The trial account only allows you to call the PDF-to-Text API up to 20 times for learning purpose. [Upgrade to a Premium plan](https://www.whatsmate.net/pdf-api-subscribe.html) to use the API seriously.


Want to extract PDF text in another programming language? Check out the [PDF-to-Text API](https://www.whatsmate.net/pdf-to-text-api.html) page.


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

