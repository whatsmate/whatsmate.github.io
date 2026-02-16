---
layout: post
title: Send PDF Files over WhatsApp in Node.js/JavaScript - Complete Guide
subtitle: Automate WhatsApp document sharing using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2026-02-12T13:45:00+08:00
---

## Automate WhatsApp Document Sharing with Node.js/JavaScript

Looking to automate PDF delivery, document notifications, or file sharing from your JavaScript applications? This guide walks you through sending PDF files to WhatsApp users using Node.js and the WhatsMate WA Gateway REST API. Perfect for JavaScript developers, full-stack engineers, and Node.js enthusiasts who want to integrate document delivery into their JavaScript-based WhatsApp messaging workflows.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate WA Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Node.js installed** - Version 12+ recommended for modern JavaScript features
4. **PDF file ready** - Have the document you want to send available locally

> ⚠️ **Important**: Recipients must register with the WhatsMate WA Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/whatsapp-gateway-api.html).


### 📝 Step-by-Step Implementation

Follow these steps to send your first PDF document to a WhatsApp user from a Node.js application:


#### 1. **Copy the Node.js Code Template**
Start by copying the following source code into your JavaScript file:

<script src="https://gist.github.com/whatsmate/063d9bfcfcd13cfab9b981500c9dcd5d.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the Node.js code:

- **Lines 7-9**: Replace `YOUR_OWN_GATEWAY_INSTANCE_ID`, `YOUR_OWN_CLIENT_ID`, and `YOUR_OWN_SECRET_ID` with your WhatsApp gateway instance ID, Client ID, and Secret
- **Line 12**: Replace `12025550108` with the target phone number (including the country code)
- **Line 13**: Replace `../assets/subwaymap.pdf` with the path to your PDF file
- **Line 14**: Replace `anyname.pdf` with the desired filename for the document
- **Line 15**: Replace `Hope you like it` with an optional caption for your PDF


#### 3. **Make the Script Executable**
Set execute permissions on your script (if needed):
```bash
chmod 755 send-pdf-individual.js
```


#### 4. **Send Your PDF Document**
Run the Node.js script to deliver your PDF to WhatsApp:
```bash
./send-pdf-individual.js
```


### 🔧 Common Use Cases

This automation approach is ideal for:
- **Automated report delivery** - Send daily/weekly PDF reports to WhatsApp from Node.js applications
- **Document sharing automation** - Deliver invoices, receipts, or contracts via WhatsApp using Node.js
- **System documentation** - Share configuration files or logs as PDF documents from JavaScript systems
- **Educational content** - Distribute learning materials or tutorials through WhatsApp from Node.js apps
- **Integration with JavaScript document generation** - Combine with Node.js libraries that create PDFs for WhatsApp delivery


### 🚀 Get Started Today

Ready to automate your document sharing over WhatsApp with Node.js? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/whatsapp-gateway-api.html) and start sending PDF files within minutes!

---

**Next Steps**: Once you've mastered basic PDF sending, explore advanced features like sending [images](https://www.whatsmate.net/whatsapp-image-individual-api.html) or [group messages](https://www.whatsmate.net/whatsapp-group-message-api.html) through the WhatsMate WA Gateway API documentation.