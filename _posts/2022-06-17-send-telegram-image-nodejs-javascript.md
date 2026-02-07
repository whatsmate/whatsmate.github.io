---
layout: post
title: Send Images over Telegram in Node.js/JavaScript - Complete Guide
subtitle: Automate Telegram image sharing using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2026-01-30T22:54:01+08:00
---

## 🚀 Automate Telegram Image Sharing with Node.js/JavaScript

Looking to automate Telegram image sharing, visual notifications, or media delivery from your JavaScript applications? This guide walks you through sending images to Telegram users using Node.js and the WhatsMate Telegram Gateway REST API. Perfect for JavaScript developers, full-stack engineers, and Node.js enthusiasts who want to integrate visual content delivery into their JavaScript-based workflows.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate Telegram Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Node.js installed** - Version 12+ recommended for modern JavaScript features
4. **Basic JavaScript knowledge** - Familiarity with Node.js and JavaScript programming
5. **Image file ready** - Have the image you want to send available locally

> ⚠️ **Important**: Recipients must register with the WhatsMate Telegram Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/telegram-gateway-api.html).


### 🎥 Video Walkthrough

<iframe width="560" height="315" src="https://www.youtube.com/embed/3HADfn6roJw?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


### 📝 Step-by-Step Implementation

Follow these steps to send your first image to a Telegram user from a Node.js application:


#### 1. **Copy the Node.js Code Template**
Start by copying the following source code into your JavaScript file:

<script src="https://gist.github.com/whatsmate/31a263a342f161415aa8c1d735c1630d.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the JavaScript code:

- **Line 7**: Replace `YOUR_OWN_GATEWAY_INSTANCE_ID` with your Telegram gateway instance ID
- **Lines 8-9**: Update `YOUR_OWN_CLIENT_ID` and `YOUR_OWN_SECRET_ID` with your Client ID and Secret
- **Line 12**: Replace `12025550108` with the target phone number (including the country code)
- **Line 13**: Replace `../assets/cute-girl.jpg` with the path to your image file
- **Line 14**: Replace `Lovely Gal` with an optional caption for your image


#### 3. **Run Your Node.js Script**
Execute your JavaScript script to deliver your image to Telegram:
```bash
# Navigate to the script directory
cd nodejs

# Make the script executable (Linux/macOS)
chmod +x send-telegram-photo.js

# Run the script directly (requires shebang line)
./send-telegram-photo.js

# Or run with Node.js directly
node send-telegram-photo.js
```


### 🔧 Common Use Cases

This automation approach is ideal for:
- **Full-stack applications** - Send images to Telegram from Express.js, Nest.js, or other Node.js frameworks
- **Serverless functions** - Integrate Telegram image sharing into AWS Lambda, Azure Functions, or Google Cloud Functions
- **Microservices** - Add Telegram notifications with images to Node.js microservices
- **Automation scripts** - Use Node.js for scheduled image delivery and automation workflows
- **Real-time applications** - Deliver images via Telegram from Socket.io or WebSocket applications
- **CLI tools** - Build command-line tools that send images to Telegram


### 🚀 Get Started Today

Ready to automate your image sharing over Telegram with Node.js/JavaScript? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/telegram-gateway-api.html) and start sending images within minutes!

---

**Next Steps**: Once you've mastered basic image sending, explore advanced features like sending [documents](https://www.whatsmate.net/telegram-document-individual-api.html), [audio files](https://www.whatsmate.net/telegram-audio-individual-api.html), or [group messages](https://www.whatsmate.net/telegram-group-message-api.html) through the WhatsMate Telegram Gateway API documentation.

