---
layout: post
title: Send PDF Files over WhatsApp in C#/.NET (Visual Studio 2019) - Complete Guide
subtitle: Automate WhatsApp PDF document sharing using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2026-02-12T14:30:00+08:00
---

## 🚀 Automate WhatsApp PDF Sharing with C#/.NET and Visual Studio 2019

> ⚠️ **Visual Studio 2019 Notice**: This guide uses Visual Studio 2019 with legacy .NET libraries. For new projects, we recommend using **[Visual Studio 2022 with modern C#/.NET](/2022-07-18-send-whatsapp-pdf-c-sharp-dot-net-vs2022/)** for better performance, security, and modern features.

Looking to automate WhatsApp PDF document sharing from legacy C#/.NET applications using Visual Studio 2019? This guide walks you through sending PDF files to WhatsApp users using C# with Visual Studio 2019 and the WhatsMate WA Gateway REST API. Perfect for maintaining legacy .NET applications that require WhatsApp document delivery capabilities.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate WA Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Visual Studio 2019** - Legacy .NET development environment
4. **PDF file ready** - Have the PDF file you want to send available locally
5. **Legacy .NET libraries** - This version uses `System.Web.Script.Serialization` (requires System.Web.Extensions reference)

> ⚠️ **Important**: Recipients must register with the WhatsMate WA Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/whatsapp-gateway-api.html).


### 📝 Step-by-Step Implementation

Follow these steps to send your first PDF file to a WhatsApp user from a legacy C# application using Visual Studio 2019:


#### 1. **Copy the C# Code Template**
Start by copying the following source code into your C# file:

<script src="https://gist.github.com/whatsmate/93ed36e28cbc73495d6ad1862cf61193.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the C# code:

- **Line 10**: Replace `YOUR_INSTANCE_ID` with your WhatsApp gateway instance ID
- **Lines 11-12**: Update `YOUR_CLIENT_ID_HERE` and `YOUR_CLIENT_SECRET_HERE` with your Client ID and Secret
- **Line 20**: Replace `12025550105` with the target phone number (including the country code)
- **Line 22**: Replace `C:\\TEMP\\subwaymap.pdf` with the path to your PDF file
- **Line 23**: Replace `anyname.pdf` with your preferred filename for the recipient
- **Line 24**: Replace `You will find the map handy.` with your desired caption


#### 3. **Add Required Reference**
In Visual Studio 2019, ensure you have the `System.Web.Extensions` reference added:
1. Right-click your project → **Add Reference**
2. Go to **Assemblies** → **Framework**
3. Check **System.Web.Extensions**
4. Click **OK**


#### 4. **Send Your PDF**
Build and run your C# application in Visual Studio 2019 to deliver your PDF to WhatsApp:
1. Press **F5** to build and run in debug mode
2. Or use **Ctrl+F5** to run without debugging
3. Check the console output for success confirmation


### 🔧 Common Use Cases

This legacy automation approach is ideal for:
- **Maintaining legacy Windows applications** - Send PDF reports to WhatsApp from older Windows Forms or WPF apps
- **Legacy ASP.NET web applications** - Integrate WhatsApp PDF sharing into older ASP.NET web apps
- **Legacy system integration** - Connect older .NET Framework applications to modern WhatsApp messaging
- **Business reporting for legacy systems** - Automatically send PDF reports from existing .NET Framework applications
- **Document automation for legacy workflows** - Generate and send PDF documents from legacy Office automation systems


### 🚀 Get Started Today

Ready to automate your PDF sharing over WhatsApp with legacy C#/.NET and Visual Studio 2019? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/whatsapp-gateway-api.html) and start sending PDF documents within minutes!

---

**Next Steps**: 
- **For new projects**: Use **[Visual Studio 2022 with modern C#/.NET](/2022-07-18-send-whatsapp-pdf-c-sharp-dot-net-vs2022/)** for better performance and modern features
- **Explore advanced features**: Once you've mastered basic PDF sending, explore sending [images](https://www.whatsmate.net/whatsapp-image-individual-api.html) or [group messages](https://www.whatsmate.net/whatsapp-group-message-api.html) through the WhatsMate WA Gateway API documentation.