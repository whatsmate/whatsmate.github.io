---
layout: post
title: How to Convert a PDF file to text in Node.js
subtitle: Using the WhatsMate PDF-to-Text REST API
published: true
last_modified_at: 2026-01-28T20:11:00+08:00
---

This article shows you how to extract text from an online PDF document in `Node.js`.


Here's how:

1. Copy the following source code to your `Node.js` script.  <script src="https://gist.github.com/whatsmate/029ea4925c99b72eb881fb65596d7ece.js"></script>
2. Specify the URL of your online PDF document on line 10.
3. Replace the Client ID and Secret on lines 5 and 6 if you have your own credentials.
6. Make your script executable: `chmod 755 extract-pdf-text-sync.js`
7. Run the script to see the result: `./extract-pdf-text-sync.js`


If your PDF file is larger than 1 MB, you will need to call the asynchronous API instead. See an <a href="https://github.com/whatsmate/pdf-demos/tree/master/nodejs">example in Node.js</a>.



The trial account only allows you to call the PDF-to-Text API up to 20 times for learning purpose. [Upgrade to a Premium plan](https://www.whatsmate.net/pdf-api-subscribe.html) to use the API seriously.


Want to extract PDF text in another programming language? Check out the [PDF-to-Text API](https://www.whatsmate.net/pdf-to-text-api.html) page.


<br>

