---
layout: post
title: Translate Text in Node.js - Complete Guide
subtitle: Automate translations using the WhatsMate Translation REST API
redirect_from:
  - /2016-08-18-translate-text-nodejs/
published: true
last_modified_at: 2026-03-12T11:05:09+08:00
---

## Automate Text Translation with Node.js

Need to translate text programmatically in your Node.js applications? This guide walks you through translating text using Node.js and the WhatsMate Translation REST API. Perfect for JavaScript developers, backend engineers, and anyone who wants to integrate automatic translations into their Node.js projects.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **Node.js installed** - Node.js runtime environment
2. **Language codes** - Know the ISO language codes for source and target languages


> ℹ️ **Note**: The trial account allows up to 10 translation API calls for learning purposes. [Subscribe to a Premium plan](https://www.whatsmate.net/translation-subscribe.html) for production use.


### 🎥 Video Walkthrough

<iframe width="560" height="315" src="https://www.youtube.com/embed/5OkcpJFSCHc?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


### 📝 Step-by-Step Implementation

Follow these steps to perform your first text translation in Node.js:


#### 1. **Copy the Script Template**
Start by copying the following source code into your JavaScript file:

{% include gist-styles.html %}

<script src="https://gist.github.com/whatsmate/41edc6a2330eb3f78eb86360ea195e38.js"></script>


#### 2. **Configure the Parameters**
Customize these key parameters in the script:

- **Line 10**: Replace with the source language code (e.g., `en` for English)
- **Line 11**: Replace with the target language code (e.g., `de` for German)
- **Line 12**: Provide the text you want to translate


> 🔍 **Looking for language codes?** See the [complete listing of supported language codes](http://api.whatsmate.net/v1/translation/supported-codes).


#### 3. **Make the Script Executable**
Set execute permissions on your script:
```bash
chmod 755 translate-text.js
```


#### 4. **Run the Translation**
Execute the script to see the translated result:
```bash
./translate-text.js
```


### 🔧 Common Use Cases

This automation approach is ideal for:
- **Web applications** - Translate content for international website visitors
- **API services** - Add translation endpoints to your REST APIs
- **Chatbots** - Translate messages in real-time conversations
- **Content processing** - Translate user-generated content automatically
- **Microservices** - Build translation services for distributed systems


### 🚀 Get Started Today

Ready to automate your text translations? You'll need an account to access the API. [Sign up for a Premium plan](https://www.whatsmate.net/translation-subscribe.html) and start translating within minutes!

---

**Next Steps**: Once you've mastered basic text translation, explore translating text in other programming languages through the [Translation API Getting Started Guide](https://www.whatsmate.net/translation-api.html).

