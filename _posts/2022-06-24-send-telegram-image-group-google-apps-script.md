---
layout: post
title: Send Images to Telegram Groups from Google Apps Script - Complete Guide
subtitle: Automate Telegram group image sharing using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2026-02-06T20:30:00+08:00
---

## 🚀 Automate Telegram Group Image Sharing with Google Apps Script

Need to integrate Telegram group image sharing into your Google Workspace automation, Sheets workflows, or Drive-based processes? This guide shows you how to deliver images to Telegram groups using Google Apps Script and the WhatsMate Telegram Gateway REST API. Perfect for Google Workspace users automating business processes, data workflows, or team collaboration that needs visual content delivery to group chats.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate Telegram Gateway account** - Required for API access
2. **Group membership** - The gateway must be a member of the target Telegram group
3. **Google account with Drive access** - To store and access image files
4. **Image file in Google Drive** - Have the image you want to send uploaded to your Drive
5. **Basic Google Apps Script knowledge** - Familiarity with script editor and functions

> ⚠️ **Important**: The gateway must be a member of the Telegram group you want to send messages to. The group admin phone number is used to uniquely identify the group.

> 📁 **File Requirement**: The image file must be uniquely named and exist in your Google Drive. The script searches for files by name, so ensure your filename is unique.


### 📝 Step-by-Step Implementation

Follow these steps to send your first image to a Telegram group from Google Apps Script:


#### 1. **Set Up Google Apps Script Project**
Create a new Google Apps Script project:

1. **Open Google Apps Script**: Go to [script.google.com](https://script.google.com)
2. **Create new project**: Click "New Project"


#### 2. **Copy the Google Apps Script Source Code**
Copy the following source code into your Google Apps Script file, replacing the default code:

<script src="https://gist.github.com/whatsmate/e20ad3099671749fe14df789fa4702e0.js"></script>

3. **Save the project**: Click the save icon or press `Ctrl+S`


#### 3. **Configure a few Parameters**
Customize these key parameters in the Google Apps Script code:

- **Line 3**: Replace `"Muscle Men Club"` with the name of your target Telegram group
- **Line 4**: Replace `"12025550108"` with the phone number of the group admin (including country code)
- **Line 5**: Replace `"butterfly_flower.jpg"` with the exact filename of your image in Google Drive
- **Line 6**: Replace `"Beautiful"` with an optional caption for your image
- **Line 19**: Replace `"YOUR_INSTANCE_ID_HERE"` with your Telegram gateway instance ID
- **Line 20**: Replace `"YOUR_CLIENT_ID_HERE"` with your Client ID
- **Line 21**: Replace `"YOUR_CLIENT_SECRET_HERE"` with your Client Secret
- **Line 47**: **Important**: Also update this line to match your image filename


#### 4. **Upload Image to Google Drive**
Ensure your image file is uploaded to Google Drive with the exact filename specified in the script.


#### 5. **Run the Script**
Execute the script to send your image:

1. **Select function**: Choose `demoSendTelegramImageToGroupFromDrive` from the function dropdown
2. **Run the script**: Click the play (▶) button
3. **Review logs**: Check the execution log for success messages or errors
4. **Authorize if prompted**: Grant necessary permissions for Drive access and URL fetching


### 🔧 Common Use Cases

This Google Apps Script integration is ideal for:
- **Google Sheets automation** - Send charts, graphs, or data visualizations from Sheets to Telegram groups
- **Google Forms processing** - Automatically send uploaded images from Forms to Telegram groups
- **Drive-based workflows** - Trigger image delivery when files are added to specific Drive folders
- **Google Workspace automation** - Integrate with Gmail, Calendar, or Docs for automated image sharing
- **Business process automation** - Schedule regular image delivery from Drive-based reports to team groups


### 🚀 Get Started Today

Ready to integrate Telegram group image sharing into your Google Workspace automation? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/telegram-gateway-api.html) and start sending images to groups from your Google Apps Script within minutes!

---

**Next Steps**: Once you've mastered group image sending, explore advanced features like sending [documents to groups](https://www.whatsmate.net/telegram-group-document-api.html), [audio files to groups](https://www.whatsmate.net/telegram-group-audio-api.html), or [individual messages](https://www.whatsmate.net/telegram-gateway-api.html) through the WhatsMate Telegram Gateway API documentation.

