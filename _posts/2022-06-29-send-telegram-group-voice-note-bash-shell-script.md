---
layout: post
title: Send Voice Note Files to Telegram Groups from Shell Script - Complete Guide
subtitle: Automate Telegram group voice note sharing using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2026-02-07T08:45:00+08:00
---

## 🚀 Automate Telegram Group Voice Note Sharing with Shell Scripts

Need to deliver voice notes, audio recordings, or voice messages to Telegram groups directly from your terminal? This guide walks you through sending voice note files (OPUS format) to Telegram groups using a simple shell script and the WhatsMate Telegram Gateway REST API. Perfect for community managers, team leaders, and automation enthusiasts who want to integrate group voice note delivery into their workflows.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate Telegram Gateway account** - Required for API access
2. **Group registration** - The Telegram group must be registered with the Gateway first
3. **Basic shell scripting knowledge** - Familiarity with terminal commands
4. **Voice note file ready** - Have the OPUS file you want to send available locally
5. **Base64 utility** - The `base64` command must be available on your system

> ⚠️ **Important**: Telegram groups must be registered with the WhatsMate Telegram Gateway before they can receive messages. Unregistered groups will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/telegram-group-message-api.html).


### 📝 Step-by-Step Implementation

Follow these steps to send your first voice note file to a Telegram group from a shell script:


#### 1. **Copy the Script Template**
Start by copying the following source code into your script file:

<script src="https://gist.github.com/whatsmate/514f055417f5724f1c2de37eadc975cf.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the script:

- **Line 13**: Replace `YOUR_OWN_INSTANCE_ID_HERE` with your Telegram gateway instance ID
- **Lines 14-15**: Update `YOUR_OWN_CLIENT_ID_HERE` and `YOUR_OWN_SECRET_HERE` with your Client ID and Secret
- **Line 18**: Replace `Muscle Men Club` with your target Telegram group name
- **Line 19**: Replace `12025550108` with the phone number of the group admin (including country code)
- **Line 20**: Replace `../assets/message.opus` with the path to your OPUS voice note file
- **Line 21**: Replace `message.opus` with the desired filename for the voice note
- **Line 22**: Replace `Listen to my voice` with an optional caption for your voice note


#### 3. **Make the Script Executable**
Set execute permissions on your script:
```bash
chmod 755 group-send-telegram-opus.sh
```


#### 4. **Send Your Voice Note File**
Run the script to deliver your voice note to the Telegram group:
```bash
./group-send-telegram-opus.sh
```


### 🔧 Common Use Cases

This automation approach is ideal for:
- **AI/TTS integration** - Generate voice messages using text-to-speech (TTS) APIs and deliver them to Telegram groups for automated announcements, notifications, or interactive voice responses
- **Group voice announcements** - Send voice updates or announcements to Telegram groups
- **Team voice notifications** - Deliver voice notifications or alerts to team collaboration groups
- **Voice message distribution** - Share voice recordings, memos, or voice messages with group members
- **Automated voice communications** - Send pre-recorded voice messages to multiple groups


### 🚀 Get Started Today

Ready to automate your group voice note sharing over Telegram? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/telegram-gateway-api.html) and start sending voice note files to groups within minutes!

---

**Next Steps**: Once you've mastered group voice note sending, explore advanced features like sending [audio files to groups](https://www.whatsmate.net/telegram-group-audio-api.html), [images to groups](https://www.whatsmate.net/telegram-group-image-api.html), [documents to groups](https://www.whatsmate.net/telegram-group-document-api.html), or [messages to individuals](https://www.whatsmate.net/telegram-gateway-api.html) through the WhatsMate Telegram Gateway API documentation.

