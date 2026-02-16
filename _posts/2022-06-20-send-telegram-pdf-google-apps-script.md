---
layout: post
title: Send PDF Files over Telegram from Google Apps Script - Complete Guide
subtitle: Automate Telegram PDF document sharing using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2026-02-04T17:21:16+0800
---

## Automate Telegram PDF Sharing with Google Apps Script

Looking to automate Telegram PDF document sharing directly from Google Workspace? This guide walks you through sending PDF files to Telegram users using Google Apps Script and the WhatsMate Telegram Gateway REST API. Perfect for Google Workspace users, spreadsheet automation enthusiasts, and anyone who wants to integrate Telegram document delivery with Google Drive, Sheets, or other Google services.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate Telegram Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Google account** - Access to Google Drive and Google Apps Script
4. **Basic JavaScript knowledge** - Familiarity with Google Apps Script (JavaScript-based)
5. **PDF in Google Drive** - Have the PDF file you want to send uploaded to your Google Drive
6. **Google Apps Script access** - Ability to create and run scripts in Google's script editor

> ⚠️ **Important**: Recipients must register with the WhatsMate Telegram Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/telegram-gateway-api.html).


### 📝 Step-by-Step Implementation

Follow these steps to send your first PDF file to a Telegram user from Google Apps Script:


#### 1. **Create a New Google Apps Script Project**
1. Go to [script.google.com](https://script.google.com)
2. Click "New Project"
3. Delete the default function and paste the following code:


#### 2. **Copy the Google Apps Script Code Template**
Copy the following source code into your Apps Script project:

<script src="https://gist.github.com/whatsmate/6d0c2d985a3a4ba9760b8bbc9a9f8e3f.js"></script>


#### 3. **Configure a few Parameters**
Customize these key parameters in the Google Apps Script code:

- **Line 3**: Replace `12025550108` with the target phone number (including the country code)
- **Line 4**: Replace `subwaymap.pdf` with the filename of your PDF in Google Drive
- **Line 5**: Replace `anyname.pdf` with your preferred filename for the recipient
- **Line 6**: Replace `Check this out` with your desired caption
- **Line 19**: Replace `YOUR_INSTANCE_ID_HERE` with your Telegram gateway instance ID
- **Lines 20-21**: Update `YOUR_CLIENT_ID_HERE` and `YOUR_CLIENT_SECRET_HERE` with your Client ID and Secret


#### 4. **Upload Your PDF to Google Drive**
1. Upload your PDF file to Google Drive
2. Ensure the filename matches exactly what you specified in the script
3. Note: The script searches for files by name, so filenames must be unique in your Drive


#### 5. **Run Your Google Apps Script**
1. Save your script project
2. Select the `demoSendTelegramPdfInDrive` function from the dropdown
3. Click the "Run" button (▶️)
4. Authorize the script when prompted (first time only)
5. Check the execution log for success confirmation


### 🔧 Common Use Cases

This automation approach is ideal for:
- **Google Sheets automation** - Send PDF reports via Telegram based on spreadsheet data or triggers
- **Google Forms responses** - Automatically send PDF documents when form submissions are received
- **Google Drive workflows** - Share PDFs from Drive folders via Telegram automatically
- **Scheduled reports** - Use time-driven triggers to send daily/weekly PDF reports
- **Business automation** - Integrate Telegram document sharing with Google Workspace business processes
- **Educational tools** - Share educational PDFs or materials via Telegram from Google Classroom workflows
- **Invoice delivery** - Automatically send PDF invoices to clients via Telegram
- **Document distribution** - Share PDF manuals, guides, or documentation with team members


### 🚀 Get Started Today

Ready to automate your PDF sharing over Telegram from Google Apps Script? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/telegram-gateway-api.html) and start sending PDF documents within minutes!

---

**Next Steps**: Once you've mastered basic PDF sending, explore advanced features like sending [images](https://www.whatsmate.net/telegram-image-individual-api.html), [audio files](https://www.whatsmate.net/telegram-audio-individual-api.html), or [group messages](https://www.whatsmate.net/telegram-group-message-api.html) through the WhatsMate Telegram Gateway API documentation.

