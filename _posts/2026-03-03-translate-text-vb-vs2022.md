---
layout: post
title: Translate Text in VB.NET using Visual Studio 2022 - Complete Guide
subtitle: Automate translations using the WhatsMate Translation REST API
published: true
last_modified_at: 2026-03-03T13:40:00+08:00
---

## Automate Text Translation with VB.NET and VS 2022

Need to translate text programmatically in your modern VB.NET applications? This guide walks you through translating text using VB.NET and the WhatsMate Translation REST API with Visual Studio 2022. Perfect for VB.NET developers building contemporary Windows applications with the latest Visual Studio IDE.

> **Note for Visual Studio 2019 users**: If you're using Visual Studio 2019, please refer to [this earlier tutorial](/2016-08-23-translate-text-vb/) instead.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **Visual Studio 2022** - Community, Professional, or Enterprise edition
2. **.NET 6.0 or higher** - Modern .NET runtime and SDK
3. **Language codes** - Know the ISO language codes for source and target languages


> ℹ️ **Note**: The trial account allows up to 10 translation API calls for learning purposes. [Subscribe to a Premium plan](https://www.whatsmate.net/translation-subscribe.html) for production use.




### 📝 Step-by-Step Implementation

Follow these steps to perform your first text translation in VB.NET with Visual Studio 2022:


#### 1. **Copy the VB.NET Template**
Start by copying the following source code to the main module in your Console Application in Visual Studio:

{% include gist-styles.html %}

<script src="https://gist.github.com/whatsmate/a6e04ab66180d7283cc2c24e006b7b08.js"></script>


#### 2. **Configure the Parameters**
Customize these key parameters in the VB.NET code:

- **Line 68**: Replace with the source language code (e.g., `en` for English)
- **Line 69**: Replace with the target language code (e.g., `es` for Spanish)
- **Line 70**: Provide the text you want to translate


> 🔍 **Looking for language codes?** See the [complete listing of supported language codes](http://api.whatsmate.net/v1/translation/supported-codes).


#### 3. **Build and Run**
Build and run your application in Visual Studio 2022 to see the translated result.


### 🔧 Common Use Cases

This VB.NET integration with Visual Studio 2022 is ideal for:
- **Modern Windows applications** - Add translation features to contemporary desktop apps
- **Cloud-native services** - Integrate translation into microservices or serverless functions
- **Enterprise modernization** - Update legacy VB.NET systems with modern .NET capabilities
- **Cross-platform development** - Create solutions that work across Windows, macOS, and Linux
- **ASP.NET Core websites** - Translate content for international visitors


### 🚀 Get Started Today

Ready to integrate text translation into your modern VB.NET applications? You'll need an account to access the API. [Sign up for a Premium plan](https://www.whatsmate.net/translation-subscribe.html) and start translating within minutes!

---

**Next Steps**: Once you've mastered basic text translation, explore translating text in other programming languages through the [Translation API Getting Started Guide](https://www.whatsmate.net/translation-api.html).

