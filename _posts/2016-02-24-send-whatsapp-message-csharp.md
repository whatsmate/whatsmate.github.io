---
layout: post
title: Send WhatsApp Messages in C# using Visual Studio 2019 - Complete Guide
subtitle: Automate WhatsApp messaging using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2026-01-28T20:11:00+08:00
---

## 🚀 Automate WhatsApp Messaging with C# .NET

Looking to integrate WhatsApp messaging into your .NET applications? This guide walks you through sending WhatsApp messages using C# and the WhatsMate WA Gateway REST API. Perfect for .NET developers building Windows applications, services, or enterprise solutions with Visual Studio 2019.

> **Note for Visual Studio 2022 users**: If you're using Visual Studio 2022, please refer to [this updated tutorial](/2022-07-18-send-whatsapp-message-csharp-vs2022/) instead.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate WA Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Visual Studio 2019** - Community, Professional, or Enterprise edition
4. **.NET Framework** - Version 4.5 or higher
5. **Basic C# knowledge** - Familiarity with Visual Studio and C# development

> ⚠️ **Important**: Recipients must register with the WhatsMate WA Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/whatsapp-gateway-api.html).


### 🎥 Video Walkthrough

<iframe width="560" height="315" src="https://www.youtube.com/embed/9A7gtNC-_PU?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


### 📝 Step-by-Step Implementation

Follow these steps to send your first WhatsApp message from a C# application:


#### 1. **Copy the C# Template**
Start by copying the following source code to the main class in your Console Application in Visual Studio:

<script src="https://gist.github.com/whatsmate/50e30fb8c2873f5da63e.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the C# code:

- **Line 10**: Replace with your gateway instance ID
- **Lines 11-12**: Update with your Client ID and Secret
- **Line 19**: Specify the target phone number (including the country code) and your message content


#### 3. **Add Required Reference**
Add the "System.Web.Extensions" reference to your project:

1. Right-click on your project node in the Solution Explorer panel
2. Choose "Add" → "Reference..."
3. Select "Framework" on the left pane
4. Find "System.Web.Extensions" in the middle pane and check the checkbox
5. Click OK to add the reference


#### 4. **Build and Run**
Build and run your application in Visual Studio to deliver your WhatsApp message.


### 🔧 Common Use Cases

This C# integration approach is ideal for:
- **Windows desktop applications** - Add messaging features to WinForms or WPF apps
- **Windows services** - Send notifications from background services
- **Enterprise systems** - Integrate WhatsApp into business applications
- **Automated workflows** - Trigger messages from scheduled tasks or events


### 🚀 Get Started Today

Ready to integrate WhatsApp messaging into your .NET applications? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/whatsapp-gateway-api.html) and start sending messages within minutes!

---

**Next Steps**: Once you've mastered basic message sending, explore advanced features like sending images, documents, or group messages through the WhatsMate API documentation.

