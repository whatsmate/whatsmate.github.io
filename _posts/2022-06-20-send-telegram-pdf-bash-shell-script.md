---
layout: post
title: Send PDF Files over Telegram from Shell Script - Complete Guide
subtitle: Automate Telegram document sharing using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2026-02-04T16:54:01+08:00
---

## Automate Telegram Document Sharing with Shell Scripts

Looking to automate PDF delivery, document notifications, or file sharing directly from your terminal? This guide walks you through sending PDF files to Telegram users using a simple shell script and the WhatsMate Telegram Gateway REST API. Perfect for system administrators, developers, and automation enthusiasts who want to integrate document delivery into their workflows.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate Telegram Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Basic shell scripting knowledge** - Familiarity with terminal commands
4. **PDF file ready** - Have the document you want to send available locally
5. **Base64 utility** - The `base64` command must be available on your system

> ⚠️ **Important**: Recipients must register with the WhatsMate Telegram Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/telegram-gateway-api.html).


### 🎥 Video Walkthrough

<iframe width="560" height="315" src="https://www.youtube.com/embed/6yy9T7QKB94?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


### 📝 Step-by-Step Implementation

Follow these steps to send your first PDF document to a Telegram user from a shell script:


#### 1. **Copy the Script Template**
Start by copying the following source code into your script file:

<script src="https://gist.github.com/whatsmate/29929061744dc8da5940407810bedae9.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the script:

- **Line 13**: Replace `YOUR_OWN_INSTANCE_ID_HERE` with your Telegram gateway instance ID
- **Lines 14-15**: Update `YOUR_OWN_CLIENT_ID_HERE` and `YOUR_OWN_SECRET_HERE` with your Client ID and Secret
- **Line 18**: Replace `12025550108` with the target phone number (including the country code)
- **Line 19**: Replace `../assets/subwaymap.pdf` with the path to your PDF file
- **Line 20**: Replace `map.pdf` with the desired filename for the document
- **Line 21**: Replace `Check this out` with an optional caption for your PDF


#### 3. **Make the Script Executable**
Set execute permissions on your script:
```bash
chmod 755 send-telegram-pdf.sh
```


#### 4. **Send Your PDF Document**
Run the script to deliver your PDF to Telegram:
```bash
./send-telegram-pdf.sh
```


### 🔧 Common Use Cases

This automation approach is ideal for:
- **Automated report delivery** - Send daily/weekly PDF reports to Telegram
- **Document sharing automation** - Deliver invoices, receipts, or contracts via Telegram
- **System documentation** - Share configuration files or logs as PDF documents
- **Educational content** - Distribute learning materials or tutorials through Telegram
- **Integration with document generation** - Combine with scripts that create PDFs for Telegram delivery


### 🚀 Get Started Today

Ready to automate your document sharing over Telegram? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/telegram-gateway-api.html) and start sending PDF files within minutes!

---

**Next Steps**: Once you've mastered basic PDF sending, explore advanced features like sending [images](https://www.whatsmate.net/telegram-image-individual-api.html), [audio files](https://www.whatsmate.net/telegram-audio-individual-api.html), or [group messages](https://www.whatsmate.net/telegram-group-message-api.html) through the WhatsMate Telegram Gateway API documentation.

