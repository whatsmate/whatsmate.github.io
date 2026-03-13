---
layout: post
title: Translate Text in C# using Visual Studio 2019 - Complete Guide
subtitle: Automate translations using the WhatsMate Translation REST API
redirect_from:
  - /2016-08-22-translate-text-csharp/
published: true
last_modified_at: 2026-03-12T11:05:09+08:00
---

## Automate Text Translation with C# .NET

Need to translate text programmatically in your .NET applications? This guide walks you through translating text using C# and the WhatsMate Translation REST API with Visual Studio 2019. Perfect for .NET developers maintaining legacy systems or working in environments where Visual Studio 2019 is the standard.

> **💡 Recommendation**: If you're starting a new project or have the flexibility to upgrade, we strongly recommend using **Visual Studio 2022** with modern .NET 6+ for better performance, improved tooling, and long-term support. Check out our [Visual Studio 2022 tutorial](/2026-03-03-translate-text-csharp-vs2022/) for the latest approach.
>
> **This tutorial is for you if**: You need to support legacy systems, maintain existing .NET Framework applications, or work in environments where Visual Studio 2019 is the standard.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **Visual Studio 2019** - Community, Professional, or Enterprise edition
2. **.NET Framework** - Version 4.5 or higher
3. **Language codes** - Know the ISO language codes for source and target languages


> ℹ️ **Note**: The trial account allows up to 10 translation API calls for learning purposes. [Subscribe to a Premium plan](https://www.whatsmate.net/translation-subscribe.html) for production use.


### 🎥 Video Walkthrough

<iframe width="560" height="315" src="https://www.youtube.com/embed/18wHrYVH4G0?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


### 📝 Step-by-Step Implementation

Follow these steps to perform your first text translation in C#:


#### 1. **Copy the C# Template**
Start by copying the following source code to the main class in your Console Application in Visual Studio:

<script src="https://gist.github.com/whatsmate/da3c4db9d38e29a1a72c805cf34679bc.js"></script>


#### 2. **Configure the Parameters**
Customize these key parameters in the C# code:

- **Line 20**: Replace with the source language code (e.g., `en` for English)
- **Line 21**: Replace with the target language code (e.g., `ta` for Tamil)
- **Line 22**: Provide the text you want to translate


> 🔍 **Looking for language codes?** See the [complete listing of supported language codes](http://api.whatsmate.net/v1/translation/supported-codes).


#### 3. **Add Required Reference**
Add the `System.Web.Extensions` reference to your project:

1. Right-click on your project node in the Solution Explorer panel
2. Choose **Add** → **Reference...**
3. Select **Framework** on the left pane
4. Find **System.Web.Extensions** in the middle pane and check the checkbox
5. Click **OK** to add the reference


#### 4. **Build and Run**
Build and run your application in Visual Studio to see the translated result.


### 🔧 Common Use Cases

This C# integration approach is ideal for:
- **Windows desktop applications** - Add translation features to WinForms or WPF apps
- **Windows services** - Translate content from background services
- **Enterprise systems** - Integrate translation into business applications
- **ASP.NET websites** - Translate content for international visitors
- **Business intelligence tools** - Translate reports and dashboards


### 🚀 Get Started Today

Ready to integrate text translation into your .NET applications? You'll need an account to access the API. [Sign up for a Premium plan](https://www.whatsmate.net/translation-subscribe.html) and start translating within minutes!

---

**Next Steps**: Once you've mastered basic text translation, explore translating text in other programming languages through the [Translation API Getting Started Guide](https://www.whatsmate.net/translation-api.html).

