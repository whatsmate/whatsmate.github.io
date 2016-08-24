---
layout: post
title: How to translate natural languages in VB.NET
subtitle: Using the WhatsMate Translation REST API
published: true
---

This article shows you how to translate textual natural languages in Microsoft's .net language: VB.


To translate text (e.g. from English to Japanese) in VB.NET, do this:

1. Copy the following source code to the main module file in your Console Application in Visual Studio.  <script src="https://gist.github.com/whatsmate/87ab01d11a0e3184043bb558721046d8.js"></script>
2. Specify your translation requirements on lines 63 through 65. 
3. Add the reference "System.Web.Extensions" by doing this:
   1. Right-click on your project node in the Solution Explorer panel.
   2. Choose "Add" -> "Reference..."
   3. Choose "Framework" on the left pane.
   4. Look for "System.Web.Extensions" in the middle pane. Check the checkbox in front of it.
   5. Click OK.
4. Build and run the application in Visual Studio.


Looking for your language code? See the <a target="_blank" href="http://api.whatsmate.net/v1/translation/supported-codes">complete listing</a>.


The trial account only allows you to call the translation API up to 10 times for learning purpose. [Subscribe to a Premium plan](http://www.whatsmate.net/translation-subscribe.html) to use the translation API seriously.


Want to translate text in another programming language? Check out the [Translation API](http://www.whatsmate.net/translation-api.html) page.

