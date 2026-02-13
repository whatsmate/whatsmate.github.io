---
layout: post
title: Send WhatsApp Group Messages from Shell Script - Complete Guide
subtitle: Automate WhatsApp group messaging using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2026-02-13T14:30:00+08:00
---

## 🚀 Automate WhatsApp Group Messaging with Shell Script

Looking to integrate WhatsApp group messaging into your Unix/Linux automation scripts? This guide walks you through sending WhatsApp group messages using shell script and the WhatsMate WA Gateway REST API. Perfect for system administrators, DevOps engineers, or anyone using bash scripting for automation that needs WhatsApp group notifications.

### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate WA Gateway Forever Green account** - Required for group messaging API access
2. **Group setup** - Create a WhatsApp group with a unique name and add the gateway
3. **Unix/Linux system with curl** - Shell script requires bash and curl command

> ⚠️ **Important**: You need a Forever Green account to send messages to WhatsApp groups. The gateway must be added to your WhatsApp group before it can send messages. [Sign up for a Forever Green account](https://www.whatsmate.net/whatsapp-group-message-api.html) to enable group messaging capabilities.

### 📝 Step-by-Step Implementation

Follow these steps to send your first WhatsApp group message from a shell script:

#### 1. **Prepare Your WhatsApp Group**
Before coding, set up your WhatsApp group:

1. Create a new group in WhatsApp with a **unique name** (the API won't work if the name isn't unique)
2. Add the secret gateway number to the group
3. Send a "Hi" message (or any message) in the group from your personal WhatsApp account - this helps the gateway silently recognize the new group in the background

#### 2. **Copy the Shell Script Template**
Copy the following source code to your shell script:

<script src="https://gist.github.com/whatsmate/cc781206fc77896813a9e32f7707ebad.js"></script>

#### 3. **Configure Key Parameters**
Customize these essential parameters in the shell script:

- **Line 3**: Replace `YOUR_INSTANCE_ID_HERE` with your WhatsApp gateway instance ID
- **Lines 4-5**: Update `YOUR_CLIENT_ID_HERE` and `YOUR_CLIENT_SECRET_HERE` with your Forever Green Client ID and Secret
- **Line 10**: Specify the group admin's phone number (including country code, e.g., `12025550108`)
- **Line 11**: Provide your group name (must be unique)
- **Line 12**: Enter your message content

#### 4. **Make Script Executable and Run**
1. Make your shell script executable: `chmod 755 send-whatsapp-group-message.sh`
2. Run the script to send your message: `./send-whatsapp-group-message.sh`

### 🔧 Common Use Cases

This shell script integration is ideal for:
- **Team notifications** - Send automated alerts to project teams or departments
- **Event coordination** - Automate event reminders and updates
- **Business communications** - Send business updates to team WhatsApp groups
- **System monitoring** - Get group alerts for server issues or maintenance

### 🚀 Get Started Today

Ready to integrate WhatsApp group messaging into your shell scripts? You'll need a Forever Green account to access the group messaging API. [Sign up for a Forever Green account](https://www.whatsmate.net/whatsapp-group-message-api.html) and start sending group messages within minutes!

---

**Next Steps**: Once you've mastered basic group text messaging, explore advanced features like sending [images](https://www.whatsmate.net/whatsapp-group-image-api.html) or [documents](https://www.whatsmate.net/whatsapp-group-document-api.html) to WhatsApp groups through the WhatsMate WA Gateway API documentation.

