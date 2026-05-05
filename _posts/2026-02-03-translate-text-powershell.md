---
layout: post
title: Translate Text in PowerShell - Complete Guide
subtitle: Automate translations using the WhatsMate Translation REST API
redirect_from:
  - /2016-08-20-translate-text-powershell/
published: true
last_modified_at: 2026-03-12T11:05:09+08:00
---

## Automate Text Translation with PowerShell

Need to translate text programmatically in your PowerShell scripts? This guide walks you through translating text using PowerShell and the WhatsMate Translation REST API. Perfect for system administrators, DevOps engineers, and IT professionals who want to integrate automatic translations into their automation workflows.


### Prerequisites

Before you begin, ensure you have:

1. **PowerShell** - Version 5.1 or higher (PowerShell 7+ recommended)
2. **Language codes** - Know the ISO language codes for source and target languages


> **Note**: The trial account allows up to 10 translation API calls for learning purposes. [Subscribe to a Premium plan](https://www.whatsmate.net/translation-subscribe.html) for production use.


### Video Walkthrough

<iframe width="560" height="315" src="https://www.youtube.com/embed/fn3vROajsOE?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


### Step-by-Step Implementation

Follow these steps to perform your first text translation in PowerShell:


#### 1. **Copy the Script Template**
Start by copying the following source code into your PowerShell script file:

{% include gist-styles.html %}

<script src="https://gist.github.com/whatsmate/6b1455f6bba7150eedbdf6c161c089e9.js"></script>


#### 2. **Configure the Parameters**
Customize these key parameters in the script:

- **Line 6**: Replace with the source language code (e.g., `en` for English)
- **Line 7**: Replace with the target language code (e.g., `fr` for French)
- **Line 8**: Provide the text you want to translate


> **Looking for language codes?** See the [complete listing of supported language codes](http://api.whatsmate.net/v1/translation/supported-codes).


#### 3. **Run the Translation**
Execute the script in PowerShell to see the translated result:
```powershell
.\translate-text.ps1
```


### Common Use Cases

This automation approach is ideal for:
- **System administration** - Translate system alerts and notifications
- **DevOps pipelines** - Translate build/deployment messages for international teams
- **IT automation** - Add translation to PowerShell scripts and runbooks
- **Log processing** - Translate log entries or error messages
- **Scheduled tasks** - Integrate translation into automated workflows


### Get Started Today

Ready to automate your text translations? You'll need an account to access the API. [Sign up for a Premium plan](https://www.whatsmate.net/translation-subscribe.html) and start translating within minutes!

---

**Next Steps**: Once you've mastered basic text translation, explore translating text in other programming languages through the [Translation API Getting Started Guide](https://www.whatsmate.net/translation-api.html).

