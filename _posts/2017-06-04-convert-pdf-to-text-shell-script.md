---
layout: post
title: How to Convert a PDF file to text in Shell Script
subtitle: Using the WhatsMate PDF-to-Text REST API
published: true
last_modified_at: 2019-12-06T00:00:00+08:00
---

This article shows you how to extract text from an online PDF document using a shell script.


Here's how:

1. Copy the following source code to your script.  <script src="https://gist.github.com/whatsmate/6c46d5630b8e154db9600b4457b90837.js"></script>
2. Specify the URL of your online PDF document on line 9.
3. Replace the Client ID and Secret on lines 4 and 5 if you have your own credentials.
5. Make your script executable: `chmod 755 extract-pdf-text-sync.sh`
6. Run the script to see the result: `./extract-pdf-text-sync.sh`


If your PDF file is larger than 1 MB, you will need to call the asynchronous API instead. See an <a href="https://github.com/whatsmate/pdf-demos/tree/master/bash">example in Shell Script</a>. 


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

