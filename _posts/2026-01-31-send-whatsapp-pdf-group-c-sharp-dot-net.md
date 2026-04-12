---
layout: post
title: Send PDF Files to WhatsApp Groups in C#/.NET using Visual Studio 2019 - Legacy Guide
subtitle: Automate WhatsApp group document sharing using the WhatsMate WA Gateway REST API
redirect_from:
  - /2018-01-23-send-whatsapp-pdf-group-c-sharp-dot-net/
published: true
last_modified_at: 2026-03-12T11:05:09+08:00
---

## Automate WhatsApp Group Document Sharing with Legacy C#/.NET and Visual Studio 2019

Need to integrate WhatsApp group PDF sharing into legacy .NET applications for enterprise reporting, business workflows, or Windows automation? This legacy guide shows you how to deliver PDF documents to WhatsApp groups using C# and the WhatsMate WA Gateway REST API with Visual Studio 2019. Perfect for .NET developers maintaining legacy applications or using older Visual Studio versions.

> **⚠️ Legacy Notice**: This guide uses Visual Studio 2019 and legacy .NET libraries. For modern development with Visual Studio 2022, updated .NET features, and better performance, please use our **[updated Visual Studio 2022 tutorial](/2022-07-18-send-whatsapp-pdf-group-c-sharp-dot-net-vs2022/)** instead.

### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate WA Gateway Forever Green account** - Required for group messaging API access
2. **Group setup** - Create a WhatsApp group with a unique name and add the gateway
3. **Visual Studio 2019** - .NET development environment (or compatible IDE)
4. **.NET Framework 4.5 or higher** - Legacy .NET runtime
5. **PDF file ready** - Have the document you want to send available locally
6. **System.Web.Extensions reference** - Required for JSON serialization in legacy .NET

> ⚠️ **Important**: You need a Forever Green account to send messages to WhatsApp groups. The gateway must be added to your WhatsApp group before it can send messages. [Sign up for a Forever Green account](https://www.whatsmate.net/whatsapp-group-message-api.html) to enable group messaging capabilities.

### 📝 Step-by-Step Implementation

Follow these steps to send your first PDF document to a WhatsApp group from a legacy C# application in Visual Studio 2019:

#### 1. **Prepare Your WhatsApp Group**
Before coding, set up your WhatsApp group:

1. Create a new group in WhatsApp with a **unique name** (the API won't work if the name isn't unique)
2. Add the secret gateway number to the group
3. Send a "Hi" message (or any message) in the group from your personal WhatsApp account - this helps the gateway silently recognize the new group in the background

#### 2. **Set Up Visual Studio 2019 Project**
1. Open Visual Studio 2019 and create a new Console Application (.NET Framework 4.5 or higher)
2. Add reference to `System.Web.Extensions` for JSON serialization:
   - Right-click References → Add Reference
   - Select Assemblies → Framework
   - Check `System.Web.Extensions` and click OK

#### 3. **Copy the C# Source Code**
Replace the contents of your main Program.cs file with the following legacy C# source code:

{% include gist-styles.html %}

<script src="https://gist.github.com/whatsmate/9bb8f3301054d7c739a011303f9513c5.js"></script>

#### 4. **Configure Key Parameters**
Customize these essential parameters in the C# program:

- **Line 10**: Replace `YOUR_INSTANCE_ID` with your WhatsApp gateway instance ID
- **Lines 11-12**: Update `YOUR_CLIENT_ID_HERE` and `YOUR_CLIENT_SECRET_HERE` with your Forever Green Client ID and Secret
- **Line 20**: Specify your group name (must be unique)
- **Line 22**: Replace `"C:\\TEMP\\subwaymap.pdf"` with the full path to your PDF file
- **Line 23**: Replace `"anyname.pdf"` with the desired filename for the document
- **Line 24**: Replace `"You will find the map handy."` with an optional caption for your PDF

#### 5. **Prepare Your PDF File**
1. Copy your PDF file to the location specified in line 22 (default: `C:\TEMP\subwaymap.pdf`)
2. Ensure the application has read permissions for the PDF file
3. If using the sample code package, copy the PDF from `..\assets\subwaymap.pdf` to `C:\TEMP\` or your specified location

#### 6. **Build and Run**
1. Build your C# project in Visual Studio 2019 (Build → Build Solution)
2. Run the application (Debug → Start Without Debugging or F5)
3. The console will display the API response and wait for you to press Enter

### 🔧 Common Use Cases (Legacy Systems)

This legacy C# integration with Visual Studio 2019 is for maintaining existing systems and is ideal for:
- **Legacy Windows desktop applications** - Maintain WhatsApp group PDF sharing in existing WinForms or WPF applications
- **Older .NET backend services** - Support legacy ASP.NET web services or Windows services with PDF document delivery
- **Enterprise business applications** - Maintain PDF report delivery in legacy CRM, ERP, or business intelligence systems
- **System migration projects** - Maintain PDF functionality during transition from older .NET versions
- **Historical codebases** - Support maintenance of .NET Framework applications that cannot be immediately upgraded

### 🚀 Get Started Today (For Legacy Systems Only)

Ready to maintain WhatsApp group PDF sharing in your legacy C# .NET applications? You'll need a Forever Green account to access the group messaging API. [Sign up for a Forever Green account](https://www.whatsmate.net/whatsapp-group-message-api.html) to enable group messaging capabilities.

**⚠️ Important Reminder**: This guide uses legacy technologies. Consider migrating to **[Visual Studio 2022](/2022-07-18-send-whatsapp-pdf-group-c-sharp-dot-net-vs2022/)** for modern .NET features, better performance, and ongoing support.

---

**Next Steps**: Once you've mastered group PDF sending, explore advanced features like sending [images to groups](https://www.whatsmate.net/whatsapp-group-image-api.html) or [individual messages](https://www.whatsmate.net/whatsapp-gateway-api.html) through the WhatsMate WA Gateway API documentation.

**Migration Recommendation**: For long-term maintainability and access to modern features, plan your migration to Visual Studio 2022 using our [Visual Studio 2022 WhatsApp group PDF sending guide](/2022-07-18-send-whatsapp-pdf-group-c-sharp-dot-net-vs2022/).
