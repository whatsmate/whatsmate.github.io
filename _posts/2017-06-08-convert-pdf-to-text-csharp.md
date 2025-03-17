---
layout: post
title: How to Convert a PDF file to text in C#
subtitle: Using the WhatsMate PDF-to-Text REST API
published: true
last_modified_at: 2025-03-16T00:00:00+08:00
---

This article shows you how to extract text from an online PDF document in Microsoft .NET language: `C#`.


<iframe width="560" height="315" src="https://www.youtube.com/embed/uCU66rDC8eA?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


Here's how:


1. Copy the following source code to the main class in your Console Application in Visual Studio.   <script src="https://gist.github.com/whatsmate/5af944ae52d075b1c3b22832e64acd9c.js"></script>
2. Customize the TODO lines:
   * Specify the URL of your online PDF file on line 19.
   * Replace the Client ID and Secret on lines 10 and 11 if you have your own credentials.
3. Add the reference "System.Web.Extensions" by doing this:
   1. Right-click on your project node in the Solution Explorer panel.
   2. Choose "Add" -> "Reference..."
   3. Choose "Framework" on the left pane.
   4. Look for "System.Web.Extensions" in the middle pane. Check the checkbox in front of it.
   5. Click OK.
4. Build and run the application in Visual Studio.


If your PDF file is larger than 1 MB, you will need to call the asynchronous API instead. See an <a href="https://github.com/whatsmate/pdf-demos/tree/master/C_sharp">example in C#</a>.



The trial account only allows you to call the PDF-to-Text API up to 20 times for learning purpose. [Upgrade to a Premium plan](https://www.whatsmate.net/pdf-api-subscribe.html) to use the API seriously.


Want to extract PDF text in another programming language? Check out the [PDF-to-Text API](https://www.whatsmate.net/pdf-to-text-api.html) page.


<br>

