---
layout: post
title: Send WhatsApp Messages from Shell Script - Complete Guide
subtitle: Automate WhatsApp messaging using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2026-01-28T20:11:00+08:00
---

## 🚀 Automate WhatsApp Messaging with Shell Scripts

Looking to automate WhatsApp notifications, alerts, or messages directly from your terminal? This guide walks you through sending WhatsApp messages using a simple shell script and the WhatsMate WA Gateway REST API. Perfect for system administrators, developers, and automation enthusiasts who want to integrate WhatsApp into their workflows.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate WA Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Basic shell scripting knowledge** - Familiarity with terminal commands

> ⚠️ **Important**: Recipients must register with the WhatsMate WA Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/whatsapp-gateway-api.html).


### 🎥 Video Walkthrough

<iframe width="560" height="315" src="https://www.youtube.com/embed/iQnzXsuywag?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


### 📝 Step-by-Step Implementation

Follow these steps to send your first WhatsApp message from a shell script:


#### 1. **Copy the Script Template**
Start by copying the following source code into your script file:

<script src="https://gist.github.com/whatsmate/10c75499502a2ededc23.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the script:

- **Line 3**: Replace with your gateway instance ID
- **Lines 4-5**: Update with your Client ID and Secret
- **Line 10**: Specify the target phone number (including the country code, e.g., `+1234567890`)
- **Line 11**: Provide your message content


#### 3. **Make the Script Executable**
Set execute permissions on your script:
```bash
chmod 755 send-whatsapp.sh
```


#### 4. **Send Your Message**
Run the script to deliver your WhatsApp message:
```bash
./send-whatsapp.sh
```


### 🔧 Common Use Cases

This automation approach is ideal for:
- **System monitoring alerts** - Get notified when servers go down
- **Scheduled reminders** - Send daily or weekly notifications
- **Automated reports** - Deliver regular updates via WhatsApp
- **Integration with cron jobs** - Combine with scheduled tasks



### 🚀 Get Started Today

Ready to automate your WhatsApp messaging? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/whatsapp-gateway-api.html) and start sending messages within minutes!

---

**Next Steps**: Once you've mastered basic message sending, explore advanced features like sending images, documents, or group messages through the WhatsMate API documentation.

