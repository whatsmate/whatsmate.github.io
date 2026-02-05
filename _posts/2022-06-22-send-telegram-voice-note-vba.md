---
layout: post
title: Send Voice Notes over Telegram from VBA/Visual Basic - Complete Guide
subtitle: Automate Telegram voice note sharing using VBA and the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2026-02-04T18:54:01+08:00
---

## 🚀 Automate Telegram Voice Note Sharing with VBA/Visual Basic

Looking to automate Telegram voice note sharing directly from Microsoft Office applications or Windows scripts? This guide walks you through sending voice note files (OPUS format) to Telegram users using VBA (Visual Basic for Applications) and the WhatsMate Telegram Gateway REST API. Perfect for Office automation specialists, Excel power users, and Windows administrators who want to integrate Telegram voice messaging with Microsoft Office, Excel, Access, or standalone VBScript files.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate Telegram Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Microsoft Office with VBA support** - Excel, Access, Word, or Outlook with VBA enabled
4. **Basic VBA knowledge** - Familiarity with Visual Basic for Applications programming
5. **Voice note file ready** - Have the OPUS file you want to send available on your Windows system
6. **Macros enabled** - Office applications need macros enabled for VBA execution

> ⚠️ **Important**: Recipients must register with the WhatsMate Telegram Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/telegram-gateway-api.html).


### 📝 Step-by-Step Implementation

Follow these steps to send your first voice note to a Telegram user from VBA:


#### 1. **Copy the VBA Code Template**
Start by copying the following source code into your VBA module:

<script src="https://gist.github.com/whatsmate/420606fb6fb273ee82af10f6167e5ad9.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the VBA code:

- **Line 6**: Update the `Main_Routine` call parameters:
  - Replace `12025550108` with the target phone number (including the country code)
  - Replace `C:\Users\Public\martin-luther-king.opus` with the path to your OPUS voice note file
  - Replace `anyname.opus` with the desired filename for the recipient
  - Replace `I have a dream` with your desired caption
- **Lines 18-20**: Update the `TelegramVoice_Send` function parameters:
  - **Line 18**: Replace `YOUR_INSTANCE_ID_HERE` with your Telegram gateway instance ID
  - **Lines 19-20**: Update `YOUR_CLIENT_ID_HERE` and `YOUR_CLIENT_SECRET_HERE` with your Client ID and Secret


#### 3. **Prepare Your Voice Note File**
1. Copy your OPUS voice note file to a location accessible by your VBA script
2. Ensure the file path in the script matches the actual location of your voice note file
3. Note: The default example uses `C:\Users\Public\martin-luther-king.opus` - adjust as needed


#### 4. **Run Your VBA Code**
1. Open the VBA editor in your Office application (Alt+F11 in Excel/Word)
2. Insert a new module and paste the code
3. Save your workbook/document with macros enabled
4. Run the `Main_Routine` subroutine to send your voice note


### 🔧 Common Use Cases

This automation approach is ideal for:
- **Excel automation** - Send voice note notifications or messages via Telegram based on spreadsheet data or calculations
- **Business process automation** - Integrate Telegram voice note sharing with Office-based business workflows
- **Reporting systems** - Send voice notifications when reports are generated or data is processed
- **Customer service automation** - Deliver voice responses or information to clients through Telegram from CRM systems
- **Scheduled voice message delivery** - Use Windows Task Scheduler with VBScript files for automated voice note sharing


### 🚀 Get Started Today

Ready to automate your voice note sharing over Telegram from VBA? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/telegram-gateway-api.html) and start sending voice notes within minutes!

---

**Next Steps**: Once you've mastered basic voice note sending, explore advanced features like sending [audio files](https://www.whatsmate.net/telegram-audio-individual-api.html), [images](https://www.whatsmate.net/telegram-image-individual-api.html), or [documents](https://www.whatsmate.net/telegram-document-individual-api.html) through the WhatsMate Telegram Gateway API documentation.