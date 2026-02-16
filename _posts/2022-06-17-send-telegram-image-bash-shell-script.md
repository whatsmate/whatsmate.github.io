---
layout: post
title: Send Images over Telegram from Shell Script - Complete Guide
subtitle: Automate Telegram image sharing using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2026-01-30T22:54:01+08:00
---

## Automate Telegram Image Sharing with Shell Scripts

Looking to automate Telegram image sharing, visual notifications, or media delivery directly from your terminal? This guide walks you through sending images to Telegram users using a simple shell script and the WhatsMate Telegram Gateway REST API. Perfect for system administrators, developers, and automation enthusiasts who want to integrate visual content delivery into their workflows.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate Telegram Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Basic shell scripting knowledge** - Familiarity with terminal commands
4. **Image file ready** - Have the image you want to send available locally

> ⚠️ **Important**: Recipients must register with the WhatsMate Telegram Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/telegram-gateway-api.html).


### 🎥 Video Walkthrough

<iframe width="560" height="315" src="https://www.youtube.com/embed/PAusLespwtk?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


### 📝 Step-by-Step Implementation

Follow these steps to send your first image to a Telegram user from a shell script:


#### 1. **Copy the Script Template**
Start by copying the following source code into your script file:

<script src="https://gist.github.com/whatsmate/806e319ac49a980045bb3e2d4c6da050.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the script:

- **Line 13**: Replace `YOUR_OWN_INSTANCE_ID_HERE` with your Telegram gateway instance ID
- **Lines 14-15**: Update `YOUR_OWN_CLIENT_ID_HERE` and `YOUR_OWN_SECRET_HERE` with your Client ID and Secret
- **Line 18**: Replace `12025550108` with the target phone number (including the country code)
- **Line 19**: Replace `../assets/cute-girl.jpg` with the path to your image file
- **Line 24**: Replace `Lovely Gal` with an optional caption for your image


#### 3. **Make the Script Executable**
Set execute permissions on your script:
```bash
chmod 755 send-telegram-image.sh
```


#### 4. **Send Your Image**
Run the script to deliver your image to Telegram:
```bash
./send-telegram-image.sh
```


### 🔧 Common Use Cases

This automation approach is ideal for:
- **Visual system monitoring** - Send server status screenshots or graphs to Telegram
- **Automated photo sharing** - Deliver daily photos or visual updates via Telegram
- **Image-based reports** - Share charts, diagrams, or visual data through Telegram
- **Media content delivery** - Distribute images as part of automated Telegram workflows
- **Integration with image processing** - Combine with scripts that generate or modify images for Telegram delivery


### 🚀 Get Started Today

Ready to automate your image sharing over Telegram? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/telegram-gateway-api.html) and start sending images within minutes!

---

**Next Steps**: Once you've mastered basic image sending, explore advanced features like sending [documents](https://www.whatsmate.net/telegram-document-individual-api.html), [audio files](https://www.whatsmate.net/telegram-audio-individual-api.html), or [group messages](https://www.whatsmate.net/telegram-group-message-api.html) through the WhatsMate Telegram Gateway API documentation.

