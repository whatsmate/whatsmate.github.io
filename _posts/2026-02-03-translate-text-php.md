---
layout: post
title: Translate Text in PHP - Complete Guide
subtitle: Automate translations using the WhatsMate Translation REST API
redirect_from:
  - /2016-08-19-translate-text-php/
published: true
last_modified_at: 2026-03-12T11:05:09+08:00
---

## Automate Text Translation with PHP

Need to translate text programmatically in your PHP applications? This guide walks you through translating text using PHP and the WhatsMate Translation REST API. Perfect for web developers, backend engineers, and anyone who wants to integrate automatic translations into their PHP projects.


### Prerequisites

Before you begin, ensure you have:

1. **PHP environment** - A web server with PHP installed
2. **Language codes** - Know the ISO language codes for source and target languages


> **Note**: The trial account allows up to 10 translation API calls for learning purposes. [Subscribe to a Premium plan](https://www.whatsmate.net/translation-subscribe.html) for production use.


### Video Walkthrough

<iframe width="560" height="315" src="https://www.youtube.com/embed/t5qDtO1FNxU?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


### Step-by-Step Implementation

Follow these steps to perform your first text translation in PHP:


#### 1. **Copy the Script Template**
Start by copying the following source code into your PHP file:

{% include gist-styles.html %}

<script src="https://gist.github.com/whatsmate/c91e4cc10093b7120b82e2341717e619.js"></script>


#### 2. **Configure the Parameters**
Customize these key parameters in the script:

- **Line 8**: Replace with the source language code (e.g., `en` for English)
- **Line 9**: Replace with the target language code (e.g., `it` for Italian)
- **Line 10**: Provide the text you want to translate


> **Looking for language codes?** See the [complete listing of supported language codes](http://api.whatsmate.net/v1/translation/supported-codes).


#### 3. **Deploy to Your Server**
Upload the PHP file to your web server in an accessible location.


#### 4. **Run the Translation**
Visit the PHP page in your browser to see the translated result.


### Common Use Cases

This automation approach is ideal for:
- **Multi-language websites** - Translate content for international visitors
- **E-commerce platforms** - Translate product descriptions and reviews
- **Customer support systems** - Translate support tickets and responses
- **Content management systems** - Automate translation of user-generated content
- **Data processing workflows** - Translate text data in batch operations


### Get Started Today

Ready to automate your text translations? You'll need an account to access the API. [Sign up for a Premium plan](https://www.whatsmate.net/translation-subscribe.html) and start translating within minutes!

---

**Next Steps**: Once you've mastered basic text translation, explore translating text in other programming languages through the [Translation API Getting Started Guide](https://www.whatsmate.net/translation-api.html).

