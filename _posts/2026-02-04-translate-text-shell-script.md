---
layout: post
title: Translate Text from Shell Script - Complete Guide
subtitle: Automate translations using the WhatsMate Translation REST API
redirect_from:
  - /2016-08-18-translate-text-shell-script/
published: true
last_modified_at: 2026-03-12T11:05:09+08:00
---

## Automate Text Translation with Shell Scripts

Need to translate text programmatically from your terminal or automation scripts? This guide walks you through translating text using a simple shell script and the WhatsMate Translation REST API. Perfect for developers, system administrators, and anyone who wants to integrate automatic translations into their workflows.


### Prerequisites

Before you begin, ensure you have:

1. **Basic shell scripting knowledge** - Familiarity with terminal commands
2. **Language codes** - Know the ISO language codes for source and target languages


> **Note**: The trial account allows up to 10 translation API calls for learning purposes. [Subscribe to a Premium plan](https://www.whatsmate.net/translation-subscribe.html) for production use.


### Video Walkthrough

<iframe width="560" height="315" src="https://www.youtube.com/embed/qeOQBpYSszA?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


### Step-by-Step Implementation

Follow these steps to perform your first text translation from a shell script:


#### 1. **Copy the Script Template**
Start by copying the following source code into your script file:

{% include gist-styles.html %}

<script src="https://gist.github.com/whatsmate/0199d2796aadff6ff8631163c1b3efcd.js"></script>


#### 2. **Configure the Parameters**
Customize these key parameters in the script:

- **Line 8**: Replace with the source language code (e.g., `en` for English)
- **Line 9**: Replace with the target language code (e.g., `id` for Indonesian)
- **Line 10**: Provide the text you want to translate


> **Looking for language codes?** See the [complete listing of supported language codes](http://api.whatsmate.net/v1/translation/supported-codes).


#### 3. **Make the Script Executable**
Set execute permissions on your script:
```bash
chmod 755 translate-text.sh
```


#### 4. **Run the Translation**
Execute the script to see the translated result:
```bash
./translate-text.sh
```


### Common Use Cases

This automation approach is ideal for:
- **Multi-language notifications** - Translate alerts for international teams
- **Content localization** - Automate translation of user-generated content
- **Data processing pipelines** - Translate text data in batch workflows
- **Customer support automation** - Translate support tickets or responses
- **Integration with cron jobs** - Schedule regular translation tasks


### Get Started Today

Ready to automate your text translations? You'll need an account to access the API. [Sign up for a Premium plan](https://www.whatsmate.net/translation-subscribe.html) and start translating within minutes!

---

**Next Steps**: Once you've mastered basic text translation, explore translating text in other programming languages through the [Translation API Getting Started Guide](https://www.whatsmate.net/translation-api.html).

