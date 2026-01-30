---
layout: post
title: Send Telegram Messages from Shell Script - Complete Guide
subtitle: Automate Telegram messaging using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2026-01-28T20:11:00+08:00
---

## 🚀 Automate Telegram Messaging with Shell Scripts

Looking to automate Telegram notifications, alerts, or messages directly from your terminal? This guide walks you through sending Telegram messages using a simple shell script and the WhatsMate Telegram Gateway REST API. Perfect for system administrators, developers, and automation enthusiasts who want to integrate Telegram into their workflows.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate Telegram Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Basic shell scripting knowledge** - Familiarity with terminal commands

> ⚠️ **Important**: Recipients must register with the WhatsMate Telegram Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/telegram-gateway-api.html).


### 🎥 Video Walkthrough

<iframe width="560" height="315" src="https://www.youtube.com/embed/tuW_WvU_NW8?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


### 📝 Step-by-Step Implementation

Follow these steps to send your first Telegram message from a shell script:


#### 1. **Copy the Script Template**
Start by copying the following source code into your script file:

<script src="https://gist.github.com/whatsmate/a29b2ba722ff34f657b002dbd0611643.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the script:

- **Line 3**: Replace with your Telegram gateway instance ID
- **Lines 4-5**: Update with your Client ID and Secret
- **Line 10**: Specify the target phone number (including the country code, e.g., `12025550108`)
- **Line 11**: Provide your message content


#### 3. **Make the Script Executable**
Set execute permissions on your script:
```bash
chmod 755 send-telegram-text.sh
```


#### 4. **Send Your Message**
Run the script to deliver your Telegram message:
```bash
./send-telegram-text.sh
```


### 🔧 Common Use Cases

This automation approach is ideal for:
- **System monitoring alerts** - Get notified when servers go down
- **Scheduled reminders** - Send daily or weekly notifications
- **Automated reports** - Deliver regular updates via Telegram
- **Integration with cron jobs** - Combine with scheduled tasks


### 🚀 Get Started Today

Ready to automate your Telegram messaging? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/telegram-gateway-api.html) and start sending messages within minutes!

---

**Next Steps**: Once you've mastered basic message sending, explore advanced features like sending [images](https://www.whatsmate.net/telegram-image-individual-api.html), [documents](https://www.whatsmate.net/telegram-document-individual-api.html), or [group messages](https://www.whatsmate.net/telegram-group-message-api.html) through the WhatsMate Telegram Gateway API documentation.



