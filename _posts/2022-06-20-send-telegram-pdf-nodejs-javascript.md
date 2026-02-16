---
layout: post
title: Send PDF Files over Telegram in Node.js/JavaScript - Complete Guide
subtitle: Automate Telegram document sharing using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2026-02-04T17:54:01+08:00
---

## Automate Telegram Document Sharing with Node.js/JavaScript

Looking to automate PDF delivery, document notifications, or file sharing from your JavaScript applications? This guide walks you through sending PDF files to Telegram users using Node.js and the WhatsMate Telegram Gateway REST API. Perfect for JavaScript developers, full-stack engineers, and Node.js enthusiasts who want to integrate document delivery into their JavaScript-based workflows.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate Telegram Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Node.js installed** - Version 12+ recommended for modern JavaScript features
4. **Basic JavaScript knowledge** - Familiarity with Node.js and JavaScript programming
5. **PDF file ready** - Have the document you want to send available locally

> ⚠️ **Important**: Recipients must register with the WhatsMate Telegram Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/telegram-gateway-api.html).


### 🎥 Video Walkthrough

<iframe width="560" height="315" src="https://www.youtube.com/embed/iFj9r08h7Rk?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


### 📝 Step-by-Step Implementation

Follow these steps to send your first PDF document to a Telegram user from a Node.js application:


#### 1. **Copy the Node.js Code Template**
Start by copying the following source code into your JavaScript file:

<script src="https://gist.github.com/whatsmate/a2e1a24fd3080e1fb0329168e582f28d.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the Node.js code:

- **Lines 7-9**: Replace `YOUR_OWN_GATEWAY_INSTANCE_ID`, `YOUR_OWN_CLIENT_ID`, and `YOUR_OWN_SECRET_ID` with your gateway instance ID, Client ID, and Secret
- **Line 12**: Replace `12025550108` with the target phone number (including the country code)
- **Line 13**: Replace `../assets/subwaymap.pdf` with the path to your PDF file
- **Line 14**: Replace `anyname.pdf` with the desired filename for the document
- **Line 15**: Replace `Check this out` with an optional caption for your PDF


#### 3. **Make the Script Executable**
Set execute permissions on your script (if needed):
```bash
chmod 755 send-telegram-pdf.js
```


#### 4. **Send Your PDF Document**
Run the Node.js script to deliver your PDF to Telegram:
```bash
./send-telegram-pdf.js
```


### 🔧 Common Use Cases

This automation approach is ideal for:
- **Automated report delivery** - Send daily/weekly PDF reports to Telegram from Node.js applications
- **Document sharing automation** - Deliver invoices, receipts, or contracts via Telegram using Node.js
- **System documentation** - Share configuration files or logs as PDF documents from JavaScript systems
- **Educational content** - Distribute learning materials or tutorials through Telegram from Node.js apps
- **Integration with JavaScript document generation** - Combine with Node.js libraries that create PDFs for Telegram delivery


### 🚀 Get Started Today

Ready to automate your document sharing over Telegram with Node.js? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/telegram-gateway-api.html) and start sending PDF files within minutes!

---

**Next Steps**: Once you've mastered basic PDF sending, explore advanced features like sending [images](https://www.whatsmate.net/telegram-image-individual-api.html), [audio files](https://www.whatsmate.net/telegram-audio-individual-api.html), or [group messages](https://www.whatsmate.net/telegram-group-message-api.html) through the WhatsMate Telegram Gateway API documentation.

