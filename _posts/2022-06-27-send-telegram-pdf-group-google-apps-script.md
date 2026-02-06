---
layout: post
title: Send PDF Files to Telegram Groups from Google Apps Script - Complete Guide
subtitle: Automate Telegram group document sharing using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2026-02-06T20:30:00+08:00
---

## 🚀 Automate Telegram Group Document Sharing from Google Workspace

Need to integrate Telegram group PDF sharing into your Google Sheets, Forms, or Docs automation workflows? This guide shows you how to deliver PDF files to Telegram groups using Google Apps Script and the WhatsMate Telegram Gateway REST API. Perfect for Google Workspace users building automation scripts, form processors, or document workflows that need PDF delivery to group chats.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate Telegram Gateway account** - Required for API access
2. **Group membership** - The gateway must be a member of the target Telegram group
3. **Google account with Drive access** - Required for Google Apps Script and file storage
4. **PDF file in Google Drive** - Have the document uploaded to your Google Drive
5. **Basic Google Apps Script knowledge** - Familiarity with script editor and functions

> ⚠️ **Important**: The gateway must be a member of the Telegram group you want to send messages to. The group admin phone number is used to uniquely identify the group.

> 📄 **Google Drive Integration**: The script automatically reads PDF files from your Google Drive, encodes them as base64, and sends them to Telegram groups. Ensure your PDF file has a unique name in Drive to avoid conflicts.


### 📝 Step-by-Step Implementation

Follow these steps to send your first PDF document to a Telegram group from Google Apps Script:


#### 1. **Set Up Google Apps Script Environment**
1. Go to [script.google.com](https://script.google.com)
2. Click "New Project" to create a blank script
3. Name your project (e.g., "Telegram PDF Sender")
4. Delete the default `myFunction` code


#### 2. **Copy the Google Apps Script Source Code**
Paste the following source code into your script editor:

<script src="https://gist.github.com/whatsmate/602ad48db2a20653bdadd81f5c9d8a08.js"></script>


#### 3. **Configure a few Parameters**
Customize these key parameters in the Google Apps Script code:

- **Line 2**: Replace `"Muscle Men Club"` with the name of your target Telegram group
- **Line 3**: Replace `"12025550108"` with the phone number of the group admin (including country code)
- **Line 4**: Replace `"subwaymap.pdf"` with the name of your PDF file in Google Drive
- **Line 5**: Replace `"anyname.pdf"` with the desired filename for the document
- **Line 6**: Replace `"Check this out"` with an optional caption for your PDF
- **Line 19**: Replace `"YOUR_INSTANCE_ID_HERE"` with your Telegram gateway instance ID
- **Line 20**: Replace `"YOUR_CLIENT_ID_HERE"` with your Client ID
- **Line 21**: Replace `"YOUR_CLIENT_SECRET_HERE"` with your Client Secret


#### 4. **Upload Your PDF to Google Drive**
1. Open [drive.google.com](https://drive.google.com)
2. Upload your PDF file or ensure it already exists in your Drive
3. Note the exact filename (including extension)


#### 5. **Run Your Google Apps Script**
1. Save your script (Ctrl+S or Cmd+S)
2. Select the `demoSendTelegramPdfToGroup` function from the dropdown menu
3. Click the "Run" button (▶️)
4. Authorize the script when prompted (first time only)
5. Check the execution log for success messages


### 🔧 Common Use Cases

This Google Apps Script integration is ideal for:
- **Google Sheets automation** - Send PDF reports generated from spreadsheet data to Telegram groups
- **Google Forms processing** - Automatically send uploaded PDFs from form submissions to Telegram groups
- **Document workflow automation** - Integrate with Google Docs, Slides, or other Workspace apps for PDF delivery
- **Scheduled reporting** - Use time-driven triggers to send regular PDF reports to Telegram groups
- **Team collaboration tools** - Add PDF sharing to team management workflows in Google Workspace


### 🚀 Get Started Today

Ready to integrate Telegram group PDF sharing into your Google Workspace automation? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/telegram-gateway-api.html) and start sending PDF documents to groups from your Google Apps Script within minutes!

---

**Next Steps**: Once you've mastered group PDF sending, explore advanced features like sending [images to groups](https://www.whatsmate.net/telegram-group-image-api.html), [audio files to groups](https://www.whatsmate.net/telegram-group-audio-api.html), or [individual messages](https://www.whatsmate.net/telegram-gateway-api.html) through the WhatsMate Telegram Gateway API documentation.

