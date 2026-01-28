---
layout: post
title: How to Convert a PDF file to text in Java
subtitle: Using the WhatsMate PDF-to-Text REST API
published: true
last_modified_at: 2026-01-28T20:11:00+08:00
---

This article shows you how to extract text from an online PDF document in `Java`.

 
<iframe width="560" height="315" src="https://www.youtube.com/embed/9JKjFL6gt2U?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


Here's how:


1. Copy the following source code to a Java file named `SyncPdfTextExtractor.java`.  <script src="https://gist.github.com/whatsmate/b9bb411ea6334fed255d034e1f6cd2cc.js"></script>
2. Specify the URL of your online PDF document on line 20.
3. Replace the Client ID and Secret on lines 10 and 11 if you have your own credentials.
4. Compile the Java file: `javac SyncPdfTextExtractor.java`
5. Execute the class to see the extracted text: `java SyncPdfTextExtractor`


If your PDF file is larger than 1 MB, you will need to call the asynchronous API instead. See an <a href="https://github.com/whatsmate/pdf-demos/tree/master/java">example in Java</a>.



The trial account only allows you to call the PDF-to-Text API up to 20 times for learning purpose. [Upgrade to a Premium plan](https://www.whatsmate.net/pdf-api-subscribe.html) to use the API seriously.


Want to extract PDF text in another programming language? Check out the [PDF-to-Text API](https://www.whatsmate.net/pdf-to-text-api.html) page.


<br>

