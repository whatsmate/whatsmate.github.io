---
layout: post
title: Send Voice Notes over Telegram from Shell Script - Complete Guide
subtitle: Automate Telegram voice note sharing using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2026-02-04T18:54:01+08:00
---

## 🚀 Automate Telegram Voice Note Sharing with Shell Scripts

Looking to automate voice message delivery, audio recordings, or spoken notifications directly from your terminal? This guide walks you through sending voice note files (OPUS format) to Telegram users using a simple shell script and the WhatsMate Telegram Gateway REST API. Perfect for system administrators, developers, and automation enthusiasts who want to integrate voice messaging into their workflows.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate Telegram Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Basic shell scripting knowledge** - Familiarity with terminal commands
4. **Voice note file ready** - Have the OPUS file you want to send available locally
5. **Base64 utility** - The `base64` command must be available on your system

> ⚠️ **Important**: Recipients must register with the WhatsMate Telegram Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/telegram-gateway-api.html).


### 📝 Step-by-Step Implementation

Follow these steps to send your first voice note to a Telegram user from a shell script:


#### 1. **Copy the Script Template**
Start by copying the following source code into your script file:

<script src="https://gist.github.com/whatsmate/04c8f9e41077a32d135936307ba3c8a9.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the script:

- **Line 13**: Replace `YOUR_OWN_INSTANCE_ID_HERE` with your Telegram gateway instance ID
- **Lines 14-15**: Update `YOUR_OWN_CLIENT_ID_HERE` and `YOUR_OWN_SECRET_HERE` with your Client ID and Secret
- **Line 18**: Replace `12025550108` with the target phone number (including the country code)
- **Line 19**: Replace `../assets/martin-luther-king.opus` with the path to your OPUS voice note file
- **Line 20**: Replace `anyname.opus` with the desired filename for the voice note
- **Line 21**: Replace `I have a dream` with an optional caption for your voice note


#### 3. **Make the Script Executable**
Set execute permissions on your script:
```bash
chmod 755 send-telegram-opus.sh
```


#### 4. **Send Your Voice Note**
Run the script to deliver your voice note to Telegram:
```bash
./send-telegram-opus.sh
```


### 🔧 Common Use Cases

This automation approach is ideal for:
- **Voice message automation** - Send pre-recorded voice messages or announcements via Telegram from system scripts
- **Audio notifications** - Deliver spoken alerts or voice notifications directly from terminal commands
- **Voice memo distribution** - Share recorded voice memos or notes with team members through Telegram
- **Language learning tools** - Distribute pronunciation examples or language lessons as voice notes
- **Customer service automation** - Send voice responses or information to clients via Telegram
- **Accessibility features** - Provide audio content for users who prefer or require voice-based communication
- **Podcast snippets** - Share short audio clips or podcast highlights as Telegram voice notes
- **Meeting recordings** - Distribute recorded meeting highlights or summaries as voice messages
- **Educational content** - Deliver lectures, tutorials, or explanations in voice format
- **System monitoring alerts** - Send voice alerts for server status or monitoring events


### 🚀 Get Started Today

Ready to automate your voice note sharing over Telegram? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/telegram-gateway-api.html) and start sending voice notes within minutes!

---

**Next Steps**: Once you've mastered basic voice note sending, explore advanced features like sending [audio files](https://www.whatsmate.net/telegram-audio-individual-api.html), [images](https://www.whatsmate.net/telegram-image-individual-api.html), or [documents](https://www.whatsmate.net/telegram-document-individual-api.html) through the WhatsMate Telegram Gateway API documentation.