---
layout: post
title: Send Images over WhatsApp from Shell Script - Complete Guide
subtitle: Automate WhatsApp image sharing using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2026-02-11T15:54:00+08:00
---

## 🚀 Automate WhatsApp Image Sharing with Shell Scripts

Looking to automate WhatsApp image sharing, visual notifications, or media delivery directly from your terminal? This guide walks you through sending images to WhatsApp users using a simple shell script and the WhatsMate WA Gateway REST API. Perfect for system administrators, developers, and automation enthusiasts who want to integrate visual content delivery into their messaging workflows.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate WA Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Basic shell scripting knowledge** - Familiarity with terminal commands
4. **Image file ready** - Have the image you want to send available locally
5. **Base64 utility** - The `base64` command must be available on your system

> ⚠️ **Important**: Recipients must register with the WhatsMate WA Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/whatsapp-gateway-api.html).


### 📝 Step-by-Step Implementation

Follow these steps to send your first image to a WhatsApp user from a shell script:


#### 1. **Copy the Script Template**
Start by copying the following source code into your script file:

<script src="https://gist.github.com/whatsmate/6b0191e083681e91ef56b4694728fdee.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the script:

- **Line 13**: Replace `YOUR_OWN_INSTANCE_ID_HERE` with your WhatsApp gateway instance ID
- **Lines 14-15**: Update `YOUR_OWN_CLIENT_ID_HERE` and `YOUR_OWN_SECRET_HERE` with your Client ID and Secret
- **Line 18**: Replace `12025550108` with the target phone number (including the country code)
- **Line 19**: Replace `../assets/cute-girl.jpg` with the path to your image file
- **Line 24**: Replace `Lovely Gal` with an optional caption for your image


#### 3. **Make the Script Executable**
Set execute permissions on your script:
```bash
chmod 755 send-whatsapp-image.sh
```


#### 4. **Send Your Image**
Run the script to deliver your image to WhatsApp:
```bash
./send-whatsapp-image.sh
```


### 🔧 Common Use Cases

This automation approach is ideal for:
- **Visual system monitoring** - Send server status screenshots or graphs to WhatsApp
- **Automated photo sharing** - Deliver daily photos or visual updates via WhatsApp
- **Image-based reports** - Share charts, diagrams, or visual data through WhatsApp
- **Media content delivery** - Distribute images as part of automated WhatsApp workflows
- **Integration with image processing** - Combine with scripts that generate or modify images for WhatsApp delivery


### 🚀 Get Started Today

Ready to automate your image sharing over WhatsApp? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/whatsapp-gateway-api.html) and start sending images within minutes!

---

**Next Steps**: Once you've mastered basic image sending, explore advanced features like sending [documents](https://www.whatsmate.net/whatsapp-document-individual-api.html) or [group messages](https://www.whatsmate.net/whatsapp-group-message-api.html) through the WhatsMate WA Gateway API documentation.