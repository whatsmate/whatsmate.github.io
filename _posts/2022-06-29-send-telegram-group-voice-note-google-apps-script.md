---
layout: post
title: Send Voice Note Files to Telegram Groups from Google Apps Script - Complete Guide
subtitle: Automate Telegram group voice note sharing using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2026-02-07T20:30:00+08:00
---

## Automate Telegram Group Voice Note Sharing with Google Apps Script

Looking to deliver voice notes, audio recordings, or spoken messages to Telegram groups directly from Google Workspace? This comprehensive guide walks you through sending voice note files (OPUS format) to Telegram groups using Google Apps Script and the WhatsMate Telegram Gateway REST API. Perfect for Google Workspace users, spreadsheet automation enthusiasts, and anyone who wants to integrate Telegram group voice messaging with Google Drive, Sheets, or other Google services.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate Telegram Gateway account** - Required for API access (sign up for a [2-week trial](https://www.whatsmate.net/telegram-gateway-api.html))
2. **Group registration** - The Telegram group must be registered with the Gateway first
3. **Google account** - Access to Google Drive and Google Apps Script
4. **Basic JavaScript knowledge** - Familiarity with Google Apps Script (JavaScript-based)
5. **Voice note file in Google Drive** - Have the OPUS file you want to send uploaded to your Google Drive

> ⚠️ **Important**: Telegram groups must be registered with the WhatsMate Telegram Gateway before they can receive messages. Unregistered groups will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/telegram-group-message-api.html).


### 📝 Step-by-Step Implementation

Follow these steps to send your first voice note file to a Telegram group from Google Apps Script:


#### 1. **Create a New Google Apps Script Project**
1. Go to [script.google.com](https://script.google.com)
2. Click "New Project"
3. Delete the default function and paste the following code:


#### 2. **Copy the Google Apps Script Code Template**
Copy the following source code into your Apps Script project:

<script src="https://gist.github.com/whatsmate/1001b29a9c5a668a89f4f9e80b574307.js"></script>


#### 3. **Configure a few Parameters**
Customize these key parameters in the Google Apps Script code:

- **Lines 2-3**: Update the `demoSendOpusToTelegramGroup` function parameters:
  - **Line 2**: Replace `Muscle Men Club` with your target Telegram group name
  - **Line 3**: Replace `12025550108` with the phone number of the group admin (including country code)
- **Line 4**: Replace `martin-luther-king.opus` with the filename of your OPUS file in Google Drive
- **Line 5**: Replace `anyname.opus` with your preferred filename for the group
- **Line 6**: Replace `I have a dream` with your desired caption
- **Lines 19-21**: Update the `sendOpusToTelegramGroup` function parameters:
  - **Line 19**: Replace `YOUR_INSTANCE_ID_HERE` with your Telegram gateway instance ID
  - **Lines 20-21**: Update `YOUR_CLIENT_ID_HERE` and `YOUR_CLIENT_SECRET_HERE` with your Client ID and Secret


#### 4. **Upload Your Voice Note File to Google Drive**
1. Upload your OPUS voice note file to Google Drive
2. Ensure the filename matches exactly what you specified in line 4 of the script
3. **Important**: The script searches for files by name, so filenames must be unique in your Drive to avoid conflicts


#### 5. **Run Your Google Apps Script**
1. Save your script project with a descriptive name (e.g., "Telegram Group Voice Note Sender")
2. Select the `demoSendOpusToTelegramGroup` function from the dropdown menu
3. Click the "Run" button (▶️)
4. Authorize the script when prompted (first time only - grants access to Google Drive and external APIs)
5. Check the execution log for success confirmation or error messages


### 🔧 Common Use Cases

This automation approach is ideal for:

- **AI/TTS integration** - Generate voice messages using text-to-speech (TTS) APIs and deliver them to Telegram groups for automated announcements, notifications, or interactive voice responses
- **Google Sheets automation** - Send voice note notifications or announcements to Telegram groups based on spreadsheet data or triggers
- **Google Forms workflows** - Automatically send voice notes to groups when form submissions are received
- **Scheduled group announcements** - Use time-driven triggers to send daily/weekly voice content to Telegram groups
- **Team collaboration tools** - Share meeting recordings, voice updates, or audio announcements with team groups from Google Workspace


### 🚀 Get Started Today

Ready to automate your group voice note sharing over Telegram from Google Apps Script? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/telegram-gateway-api.html) and start sending voice note files to groups within minutes!

---

**Next Steps**: Once you've mastered group voice note sending, explore advanced features like sending [audio files to groups](https://www.whatsmate.net/telegram-group-audio-api.html), [images to groups](https://www.whatsmate.net/telegram-group-image-api.html), [documents to groups](https://www.whatsmate.net/telegram-group-document-api.html), or [messages to individuals](https://www.whatsmate.net/telegram-gateway-api.html) through the WhatsMate Telegram Gateway API documentation.

