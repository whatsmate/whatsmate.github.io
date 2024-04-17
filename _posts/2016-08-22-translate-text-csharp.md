---
layout: post
title: How to translate natural languages in C#
subtitle: Using the WhatsMate Translation REST API
published: true
last_modified_at: 2024-04-17T00:00:00+08:00
---

This article shows you how to translate text in Microsoft's .net language: C#.


To translate textual natural languages (e.g. from English to Tamil) in C#, do this:

1. Copy the following source code to the main class in your Console Application in Visual Studio.  <script src="https://gist.github.com/whatsmate/da3c4db9d38e29a1a72c805cf34679bc.js"></script>
2. Specify your translation requirements on lines 19 through 22.
3. Add the reference "System.Web.Extensions" by doing this:
   1. Right-click on your project node in the Solution Explorer panel.
   2. Choose "Add" -> "Reference..."
   3. Choose "Framework" on the left pane.
   4. Look for "System.Web.Extensions" in the middle pane. Check the checkbox in front of it.
   5. Click OK.
4. Build and run the application in Visual Studio.


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

