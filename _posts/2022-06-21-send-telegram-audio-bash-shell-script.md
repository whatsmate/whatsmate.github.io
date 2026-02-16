---
layout: post
title: Send Audio Files over Telegram from Shell Script - Complete Guide
subtitle: Automate Telegram audio sharing using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2026-02-04T18:54:01+08:00
---

## Automate Telegram Audio Sharing with Shell Scripts

Looking to automate audio delivery, voice messages, or sound notifications directly from your terminal? This guide walks you through sending audio files (MP3 format) to Telegram users using a simple shell script and the WhatsMate Telegram Gateway REST API. Perfect for system administrators, developers, and automation enthusiasts who want to integrate audio content delivery into their workflows.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate Telegram Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Basic shell scripting knowledge** - Familiarity with terminal commands
4. **Audio file ready** - Have the MP3 file you want to send available locally
5. **Base64 utility** - The `base64` command must be available on your system

> ⚠️ **Important**: Recipients must register with the WhatsMate Telegram Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/telegram-gateway-api.html).


### 🎥 Video Walkthrough

<iframe width="560" height="315" src="https://www.youtube.com/embed/XT3IIwhT6VQ?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


### 📝 Step-by-Step Implementation

Follow these steps to send your first audio file to a Telegram user from a shell script:


#### 1. **Copy the Script Template**
Start by copying the following source code into your script file:

<script src="https://gist.github.com/whatsmate/1467e4787bfd6153f75c84f3c1d9ae21.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the script:

- **Line 13**: Replace `YOUR_OWN_INSTANCE_ID_HERE` with your Telegram gateway instance ID
- **Lines 14-15**: Update `YOUR_OWN_CLIENT_ID_HERE` and `YOUR_OWN_SECRET_HERE` with your Client ID and Secret
- **Line 18**: Replace `12025550108` with the target phone number (including the country code)
- **Line 19**: Replace `../assets/ocean-waves.mp3` with the path to your MP3 audio file
- **Line 20**: Replace `ocean.mp3` with the desired filename for the audio
- **Line 21**: Replace `Enjoy the nature` with an optional caption for your audio


#### 3. **Make the Script Executable**
Set execute permissions on your script:
```bash
chmod 755 send-telegram-mp3.sh
```


#### 4. **Send Your Audio File**
Run the script to deliver your audio to Telegram:
```bash
./send-telegram-mp3.sh
```


### 🔧 Common Use Cases

This automation approach is ideal for:
- **System monitoring alerts** - Send audio alerts for server status or monitoring events
- **Audio notifications** - Send sound alerts or voice messages to Telegram from system scripts
- **Voice message automation** - Deliver pre-recorded voice messages or announcements
- **Integration with audio processing** - Combine with scripts that generate or modify audio files for Telegram delivery
- **Automated podcast delivery** - Distribute audio content or episodes via Telegram


### 🚀 Get Started Today

Ready to automate your audio sharing over Telegram? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/telegram-gateway-api.html) and start sending audio files within minutes!

---

**Next Steps**: Once you've mastered basic audio sending, explore advanced features like sending [images](https://www.whatsmate.net/telegram-image-individual-api.html), [documents](https://www.whatsmate.net/telegram-document-individual-api.html), or [group messages](https://www.whatsmate.net/telegram-group-message-api.html) through the WhatsMate Telegram Gateway API documentation.