---
layout: post
title: Send Audio Files over Telegram from Google Apps Script - Complete Guide
subtitle: Automate Telegram audio sharing using Google Apps Script and the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2026-02-04T18:54:01+08:00
---

## 🚀 Automate Telegram Audio Sharing with Google Apps Script

Looking to automate Telegram audio file sharing directly from Google Workspace? This guide walks you through sending audio files (MP3 format) to Telegram users using Google Apps Script and the WhatsMate Telegram Gateway REST API. Perfect for Google Workspace users, spreadsheet automation enthusiasts, and anyone who wants to integrate Telegram audio delivery with Google Drive, Sheets, or other Google services.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate Telegram Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Google account** - Access to Google Drive and Google Apps Script
4. **Basic JavaScript knowledge** - Familiarity with Google Apps Script (JavaScript-based)
5. **Audio file in Google Drive** - Have the MP3 file you want to send uploaded to your Google Drive
6. **Google Apps Script access** - Ability to create and run scripts in Google's script editor

> ⚠️ **Important**: Recipients must register with the WhatsMate Telegram Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/telegram-gateway-api.html).


### 📝 Step-by-Step Implementation

Follow these steps to send your first audio file to a Telegram user from Google Apps Script:


#### 1. **Create a New Google Apps Script Project**
1. Go to [script.google.com](https://script.google.com)
2. Click "New Project"
3. Delete the default function and paste the following code:


#### 2. **Copy the Google Apps Script Code Template**
Copy the following source code into your Apps Script project:

<script src="https://gist.github.com/whatsmate/9597645f30724c02a6aace8b4a113c8b.js"></script>


#### 3. **Configure a few Parameters**
Customize these key parameters in the Google Apps Script code:

- **Lines 2-5**: Update the `demoSendTelegramMp3InDrive` function parameters:
  - **Line 2**: Replace `12025550108` with the target phone number (including the country code)
  - **Line 3**: Replace `ocean-waves.mp3` with the filename of your MP3 in Google Drive
  - **Line 4**: Replace `anyname.mp3` with your preferred filename for the recipient
  - **Line 5**: Replace `Enjoy the nature` with your desired caption
- **Lines 18-20**: Update the `sendTelegramMp3` function parameters:
  - **Line 18**: Replace `YOUR_INSTANCE_ID_HERE` with your Telegram gateway instance ID
  - **Lines 19-20**: Update `YOUR_CLIENT_ID_HERE` and `YOUR_CLIENT_SECRET_HERE` with your Client ID and Secret


#### 4. **Upload Your Audio File to Google Drive**
1. Upload your MP3 audio file to Google Drive
2. Ensure the filename matches exactly what you specified in the script
3. Note: The script searches for files by name, so filenames must be unique in your Drive


#### 5. **Run Your Google Apps Script**
1. Save your script project
2. Select the `demoSendTelegramMp3InDrive` function from the dropdown
3. Click the "Run" button (▶️)
4. Authorize the script when prompted (first time only)
5. Check the execution log for success confirmation


### 🔧 Common Use Cases

This automation approach is ideal for:
- **Google Sheets automation** - Send audio notifications or voice messages via Telegram based on spreadsheet data or triggers
- **Google Forms responses** - Automatically send audio files when form submissions are received
- **Google Drive workflows** - Share audio files from Drive folders via Telegram automatically
- **Scheduled audio delivery** - Use time-driven triggers to send daily/weekly audio content
- **Business automation** - Integrate Telegram audio sharing with Google Workspace business processes
- **Educational tools** - Share audio lessons, language recordings, or lectures via Telegram from Google Classroom workflows
- **Podcast distribution** - Automatically deliver podcast episodes to subscribers via Telegram
- **Audio content management** - Share music, sound effects, or audio recordings with team members


### 🚀 Get Started Today

Ready to automate your audio sharing over Telegram from Google Apps Script? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/telegram-gateway-api.html) and start sending audio files within minutes!

---

**Next Steps**: Once you've mastered basic audio sending, explore advanced features like sending [images](https://www.whatsmate.net/telegram-image-individual-api.html), [documents](https://www.whatsmate.net/telegram-document-individual-api.html), or [group messages](https://www.whatsmate.net/telegram-group-message-api.html) through the WhatsMate Telegram Gateway API documentation.