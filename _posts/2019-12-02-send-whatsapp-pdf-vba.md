---
layout: post
title: Send PDF Files over WhatsApp from VBA/Visual Basic - Complete Guide
subtitle: Automate WhatsApp PDF document sharing using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2026-02-12T14:00:00+08:00
---

## Automate WhatsApp PDF Sharing with VBA/Visual Basic

Looking to automate WhatsApp PDF document sharing directly from Microsoft Office applications or Windows scripts? This guide walks you through sending PDF files to WhatsApp users using VBA (Visual Basic for Applications) and the WhatsMate WA Gateway REST API. Perfect for Office automation specialists, Excel power users, and Windows administrators who want to integrate WhatsApp document delivery with Microsoft Office, Excel, Access, or standalone VBScript files.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate WA Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Microsoft Office with VBA support** - Excel, Access, Word, or Outlook with VBA enabled
4. **PDF file ready** - Have the PDF file you want to send available on your Windows system
5. **Macros enabled** - Office applications need macros enabled for VBA execution

> ⚠️ **Important**: Recipients must register with the WhatsMate WA Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/whatsapp-gateway-api.html).


### 📝 Step-by-Step Implementation

Follow these steps to send your first PDF file to a WhatsApp user from VBA:


#### 1. **Copy the VBA Code Template**
Start by copying the following source code into your VBA module or VBScript file:

<script src="https://gist.github.com/whatsmate/01ba745741b89a7394db9fa9ab845ae0.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the VBA code:

- **Line 6**: Update the `WhatsAppDoc_Send` function call parameters in `Main_Routine`:
  - Replace `12025550108` with the target phone number (including the country code)
  - Replace `C:\Users\Public\subwaymap.pdf` with the path to your PDF file
  - Replace `click_me.pdf` with your preferred filename for the recipient
  - Replace `Hope you like it.` with your desired caption
- **Line 18**: Replace `YOUR_INSTANCE_ID_HERE` with your WhatsApp gateway instance ID
- **Lines 19-20**: Update `YOUR_CLIENT_ID_HERE` and `YOUR_CLIENT_SECRET_HERE` with your Client ID and Secret


#### 3. **Prepare Your PDF File**
Copy your PDF file to a known location on your Windows system:
1. Place your PDF file in a directory like `C:\Users\Public\`
2. Ensure the file path in line 6 matches the actual location
3. Note: The VBA code includes a helper function to convert PDF files to base64 format


#### 4. **Run Your VBA Code**
Execute your VBA code to deliver your PDF to WhatsApp:

**For VBScript files:**
1. Save the code as a `.vbs` file
2. Double-click the file to run it in Windows

**For Microsoft Office VBA:**
1. Open the VBA editor (Alt+F11 in Excel/Word)
2. Insert a new module
3. Paste the code
4. Run the `Main_Routine` function from the VBA editor
5. Or call `WhatsAppDoc_Send` directly with your parameters


### 🔧 Common Use Cases

This automation approach is ideal for:
- **Excel automation** - Send PDF reports via WhatsApp based on spreadsheet data or calculations
- **Office workflows** - Automate PDF sharing from Word documents, Access databases, or Outlook emails
- **Windows scripting** - Use VBScript for scheduled PDF delivery via Windows Task Scheduler
- **Business reporting** - Automatically send PDF reports, invoices, and documents via WhatsApp from Office applications
- **Data processing** - Integrate WhatsApp PDF sharing with Excel data analysis workflows


### 🚀 Get Started Today

Ready to automate your PDF sharing over WhatsApp from VBA/Visual Basic? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/whatsapp-gateway-api.html) and start sending PDF documents within minutes!

---

**Next Steps**: Once you've mastered basic PDF sending, explore advanced features like sending [images](https://www.whatsmate.net/whatsapp-image-individual-api.html) or [group messages](https://www.whatsmate.net/whatsapp-group-message-api.html) through the WhatsMate WA Gateway API documentation.