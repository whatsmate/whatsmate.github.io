---
layout: post
title: Translate Text in C# using Visual Studio 2022 - Complete Guide
subtitle: Automate translations using the WhatsMate Translation REST API
published: true
last_modified_at: 2026-03-03T12:35:00+08:00
---

## Automate Text Translation with C# .NET and VS 2022

Need to translate text programmatically in your modern .NET applications? This guide walks you through translating text using C# and the WhatsMate Translation REST API with Visual Studio 2022. Perfect for .NET developers building contemporary Windows applications, services, or enterprise solutions with the latest Visual Studio IDE.

> **Note for Visual Studio 2019 users**: If you're using Visual Studio 2019, please refer to [this earlier tutorial](/2016-08-22-translate-text-csharp/) instead.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **Visual Studio 2022** - Community, Professional, or Enterprise edition
2. **.NET 6.0 or higher** - Modern .NET runtime and SDK
3. **Language codes** - Know the ISO language codes for source and target languages


> ℹ️ **Note**: The trial account allows up to 10 translation API calls for learning purposes. [Subscribe to a Premium plan](https://www.whatsmate.net/translation-subscribe.html) for production use.



### 📝 Step-by-Step Implementation

Follow these steps to perform your first text translation in C# with Visual Studio 2022:


#### 1. **Copy the C# Template**
Start by copying the following source code to the main class in your Console Application in Visual Studio:

<script src="https://gist.github.com/whatsmate/6346ea47a163b4cc502bc306e09721cf.js"></script>


#### 2. **Configure the Parameters**
Customize these key parameters in the C# code:

- **Line 19**: Replace with the source language code (e.g., `en` for English)
- **Line 20**: Replace with the target language code (e.g., `es` for Spanish)
- **Line 21**: Provide the text you want to translate


> 🔍 **Looking for language codes?** See the [complete listing of supported language codes](http://api.whatsmate.net/v1/translation/supported-codes).


#### 3. **Build and Run**
Build and run your application in Visual Studio 2022 to see the translated result.


### 🔧 Common Use Cases

This C# integration with Visual Studio 2022 is ideal for:
- **Modern Windows applications** - Add translation features to WinUI 3 or MAUI apps
- **Cloud-native services** - Integrate translation into microservices or serverless functions
- **Enterprise solutions** - Build business applications with modern .NET capabilities
- **Cross-platform development** - Create solutions that work across Windows, macOS, and Linux
- **ASP.NET Core websites** - Translate content for international visitors


### 🚀 Get Started Today

Ready to integrate text translation into your modern .NET applications? You'll need an account to access the API. [Sign up for a Premium plan](https://www.whatsmate.net/translation-subscribe.html) and start translating within minutes!

---

**Next Steps**: Once you've mastered basic text translation, explore translating text in other programming languages through the [Translation API Getting Started Guide](https://www.whatsmate.net/translation-api.html).

