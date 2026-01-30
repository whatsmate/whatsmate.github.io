---
layout: post
title: Send Telegram Messages from Google Apps Script - Complete Guide
subtitle: Automate Telegram messaging using Google Apps Script and the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2026-01-28T20:11:00+08:00
---

## 🚀 Automate Telegram Messaging with Google Apps Script

Looking to integrate Telegram messaging into your Google Workspace automation? This guide walks you through sending Telegram messages using Google Apps Script and the WhatsMate Telegram Gateway REST API. Perfect for Google Sheets, Docs, and Forms users who want to automate notifications and messaging directly from their Google Workspace environment.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate Telegram Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Google account** - With access to Google Apps Script
4. **Basic Google Apps Script knowledge** - Familiarity with creating and running scripts
5. **Google Workspace access** - For integrating with Sheets, Docs, or Forms

> ⚠️ **Important**: Recipients must register with the WhatsMate Telegram Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/telegram-gateway-api.html).


### 🎥 Video Walkthrough

<iframe width="560" height="315" src="https://www.youtube.com/embed/gYxliOIYqqI?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


### 📝 Step-by-Step Implementation

Follow these steps to send your first Telegram message from a Google Apps Script:


#### 1. **Copy the Google Apps Script Template**
Start by copying the following source code into your Google Apps Script project:

<script src="https://gist.github.com/whatsmate/358914cd35958847111b4bbfa380a1de.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the Google Apps Script code:

- **Line 6**: Specify the target phone number (including the country code, e.g., `12025550108`)
- **Line 9**: Provide your message content
- **Line 15**: Replace with your Telegram gateway instance ID
- **Lines 16-17**: Update with your Client ID and Secret


#### 3. **Send Your Message**
Run the `main()` function to deliver your Telegram message from your Google Apps Script project.


### 🔧 Common Use Cases

This Google Apps Script integration approach is ideal for:
- **Google Sheets automation** - Send notifications when spreadsheet data changes
- **Google Forms responses** - Automatically notify users when forms are submitted
- **Google Docs workflows** - Integrate Telegram into document collaboration
- **Scheduled Google Workspace tasks** - Combine with time-driven triggers
- **Business process automation** - Connect Telegram to Google Workspace workflows


### 🚀 Get Started Today

Ready to integrate Telegram messaging into your Google Workspace automation? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/telegram-gateway-api.html) and start sending messages within minutes!

---

**Next Steps**: Once you've mastered basic message sending, explore advanced features like sending [images](https://www.whatsmate.net/telegram-image-individual-api.html), [documents](https://www.whatsmate.net/telegram-document-individual-api.html), or [group messages](https://www.whatsmate.net/telegram-group-message-api.html) through the WhatsMate Telegram Gateway API documentation.



