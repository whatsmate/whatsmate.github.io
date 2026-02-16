---
layout: post
title: Send Images over WhatsApp in C#/.NET (Visual Studio 2019) - Legacy Guide
subtitle: Automate WhatsApp image sharing using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2026-02-11T15:54:00+08:00
---

## Automate WhatsApp Image Sharing with C#/.NET and Visual Studio 2019

Looking to automate WhatsApp image sharing, visual notifications, or media delivery from your C#/.NET applications using Visual Studio 2019? This legacy guide walks you through sending images to WhatsApp users using C# with Visual Studio 2019 and the WhatsMate WA Gateway REST API. Perfect for .NET developers maintaining legacy applications or using older Visual Studio versions.

> **⚠️ Legacy Notice**: This guide uses Visual Studio 2019 and legacy .NET libraries. For modern development with Visual Studio 2022, updated .NET features, and better performance, please use our **[updated Visual Studio 2022 tutorial](/2022-07-18-send-whatsapp-image-c-sharp-dot-net-vs2022/)** instead.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate WA Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Visual Studio 2019** - .NET development environment (or compatible IDE)
4. **Image file ready** - Have the image you want to send available locally
5. **System.Web.Extensions reference** - Required for JSON serialization in legacy .NET

> ⚠️ **Important**: Recipients must register with the WhatsMate WA Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/whatsapp-gateway-api.html).


### 📝 Step-by-Step Implementation

Follow these steps to send your first image to a WhatsApp user from a C# application using Visual Studio 2019:


#### 1. **Copy the C# Code Template**
Start by copying the following source code into your C# file:

<script src="https://gist.github.com/whatsmate/11c740b0893fb6ef4b5bde9e55e4a591.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the C# code:

- **Line 10**: Replace `YOUR_INSTANCE_ID` with your WhatsApp gateway instance ID
- **Lines 11-12**: Update `YOUR_CLIENT_ID_HERE` and `YOUR_CLIENT_SECRET_HERE` with your Client ID and Secret
- **Line 20**: Replace `12025550105` with the target phone number (including the country code)
- **Line 22**: Replace `C:\\TEMP\\cute-girl.jpg` with the path to your image file
- **Line 23**: Replace `Lovely Gal` with an optional caption for your image


#### 3. **Add Required Reference**
In Visual Studio 2019, add a reference to `System.Web.Extensions` for JSON serialization support:
1. Right-click on References in your project
2. Select "Add Reference"
3. Find and check "System.Web.Extensions"
4. Click OK


#### 4. **Send Your Image**
Build and run your C# application in Visual Studio 2019 to deliver your image to WhatsApp:
1. Press **F5** to build and run in debug mode
2. Or use **Ctrl+F5** to run without debugging
3. Check the console output for success confirmation


### 🔧 Common Use Cases

This legacy automation approach is ideal for:
- **Legacy Windows applications** - Send images to WhatsApp from older Windows Forms or WPF apps
- **Maintenance projects** - Update existing .NET applications with WhatsApp image sharing
- **Backend services** - Integrate WhatsApp image sharing into legacy ASP.NET web applications
- **Scheduled tasks** - Use Windows Task Scheduler with .NET console apps for regular image delivery
- **Business applications** - Add WhatsApp notifications with images to enterprise .NET solutions


### 🚀 Get Started Today

Ready to automate your image sharing over WhatsApp with C#/.NET and Visual Studio 2019? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/whatsapp-gateway-api.html) and start sending images within minutes!

---

**Next Steps**: Once you've mastered basic image sending, explore advanced features like sending [documents](https://www.whatsmate.net/whatsapp-document-individual-api.html) or [group messages](https://www.whatsmate.net/whatsapp-group-message-api.html) through the WhatsMate WA Gateway API documentation.

> **💡 Upgrade Recommendation**: For new projects or modern development, we strongly recommend using our **[Visual Studio 2022 tutorial](/2022-07-18-send-whatsapp-image-c-sharp-dot-net-vs2022/)** which uses modern .NET libraries, better performance, and updated development practices.