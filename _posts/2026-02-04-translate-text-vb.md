---
layout: post
title: Translate Text in VB.NET using Visual Studio 2019 - Complete Guide
subtitle: Automate translations using the WhatsMate Translation REST API
redirect_from:
  - /2016-08-23-translate-text-vb/
published: true
last_modified_at: 2026-03-12T11:05:09+08:00
---

## Automate Text Translation with VB.NET

Need to translate text programmatically in your VB.NET applications? This guide walks you through translating text using VB.NET and the WhatsMate Translation REST API with Visual Studio 2019. Perfect for VB.NET developers maintaining legacy systems or working in environments where Visual Basic is the standard.

> **Recommendation**: If you're starting a new project or have the flexibility to upgrade, we strongly recommend using **Visual Studio 2022** with modern .NET 6+ for better performance, improved tooling, and long-term support.
>
> **This tutorial is for you if**: You need to support legacy systems, maintain existing .NET Framework applications, or work in environments where VB.NET and Visual Studio 2019 are the standard.


### Prerequisites

Before you begin, ensure you have:

1. **Visual Studio 2019** - Community, Professional, or Enterprise edition
2. **.NET Framework** - Version 4.5 or higher
3. **Language codes** - Know the ISO language codes for source and target languages


> **Note**: The trial account allows up to 10 translation API calls for learning purposes. [Subscribe to a Premium plan](https://www.whatsmate.net/translation-subscribe.html) for production use.


### Step-by-Step Implementation

Follow these steps to perform your first text translation in VB.NET:


#### 1. **Copy the VB.NET Template**
Start by copying the following source code to the main module file in your Console Application in Visual Studio:

{% include gist-styles.html %}

<script src="https://gist.github.com/whatsmate/87ab01d11a0e3184043bb558721046d8.js"></script>


#### 2. **Configure the Parameters**
Customize these key parameters in the VB.NET code:

- **Line 65**: Replace with the source language code (e.g., `en` for English)
- **Line 66**: Replace with the target language code (e.g., `ja` for Japanese)
- **Line 67**: Provide the text you want to translate


> **Looking for language codes?** See the [complete listing of supported language codes](http://api.whatsmate.net/v1/translation/supported-codes).


#### 3. **Add Required Reference**
Add the `System.Web.Extensions` reference to your project:

1. Right-click on your project node in the Solution Explorer panel
2. Choose **Add** → **Reference...**
3. Select **Framework** on the left pane
4. Find **System.Web.Extensions** in the middle pane and check the checkbox
5. Click **OK** to add the reference


#### 4. **Build and Run**
Build and run your application in Visual Studio 2019 to see the translated result.


### Common Use Cases

This VB.NET integration approach is ideal for:
- **Legacy business applications** - Add translation to existing VB.NET systems
- **Windows Forms apps** - Translate content in older desktop applications
- **Enterprise systems** - Maintain translation features in established solutions
- **Government systems** - Support public sector applications still using VB.NET
- **Educational tools** - Build translation utilities for learning environments


### Get Started Today

Ready to integrate text translation into your VB.NET applications? You'll need an account to access the API. [Sign up for a Premium plan](https://www.whatsmate.net/translation-subscribe.html) and start translating within minutes!

---

**Next Steps**: Once you've mastered basic text translation, explore translating text in other programming languages through the [Translation API Getting Started Guide](https://www.whatsmate.net/translation-api.html).

