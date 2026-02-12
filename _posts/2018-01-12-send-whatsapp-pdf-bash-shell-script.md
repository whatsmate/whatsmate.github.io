---
layout: post
title: Send PDF Files over WhatsApp from Shell Script - Complete Guide
subtitle: Automate WhatsApp document sharing using the WhatsMate WhatsApp Gateway REST API
published: true
last_modified_at: 2026-02-12T12:30:00+08:00
---

## 🚀 Automate WhatsApp Document Sharing with Shell Scripts

Looking to automate PDF delivery, document notifications, or file sharing directly from your terminal? This guide walks you through sending PDF files to WhatsApp users using a simple shell script and the WhatsMate WhatsApp Gateway REST API. Perfect for system administrators, developers, and automation enthusiasts who want to integrate document delivery into their WhatsApp messaging workflows.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate WhatsApp Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Basic shell scripting knowledge** - Familiarity with terminal commands
4. **PDF file ready** - Have the document you want to send available locally
5. **Base64 utility** - The `base64` command must be available on your system

> ⚠️ **Important**: Recipients must register with the WhatsMate WhatsApp Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/whatsapp-gateway-api.html).


### 📝 Step-by-Step Implementation

Follow these steps to send your first PDF document to a WhatsApp user from a shell script:


#### 1. **Copy the Script Template**
Start by copying the following source code into your script file:

<script src="https://gist.github.com/whatsmate/66e7c6d8199848856de7650cefdc5a21.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the script:

- **Line 12**: Replace `YOUR_OWN_INSTANCE_ID_HERE` with your WhatsApp gateway instance ID
- **Lines 13-14**: Update `YOUR_OWN_CLIENT_ID_HERE` and `YOUR_OWN_SECRET_HERE` with your Client ID and Secret
- **Line 17**: Replace `12025550108` with the target phone number (including the country code)
- **Line 18**: Replace `../assets/subwaymap.pdf` with the path to your PDF file
- **Line 19**: Replace `map.pdf` with the desired filename for the document
- **Line 20**: Replace `You will find it handy.` with an optional caption for your PDF


#### 3. **Make the Script Executable**
Set execute permissions on your script:
```bash
chmod 755 send-whatsapp-pdf.sh
```


#### 4. **Send Your PDF Document**
Run the script to deliver your PDF to WhatsApp:
```bash
./send-whatsapp-pdf.sh
```


### 🔧 Common Use Cases

This automation approach is ideal for:
- **Automated report delivery** - Send daily/weekly PDF reports to WhatsApp
- **Document sharing automation** - Deliver invoices, receipts, or contracts via WhatsApp
- **System documentation** - Share configuration files or logs as PDF documents
- **Educational content** - Distribute learning materials or tutorials through WhatsApp
- **Integration with document generation** - Combine with scripts that create PDFs for WhatsApp delivery


### 🚀 Get Started Today

Ready to automate your document sharing over WhatsApp? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/whatsapp-gateway-api.html) and start sending PDF files within minutes!

---

**Next Steps**: Once you've mastered basic PDF sending, explore advanced features like sending [images](https://www.whatsmate.net/whatsapp-image-individual-api.html) or [group messages](https://www.whatsmate.net/whatsapp-group-message-api.html) through the WhatsMate WhatsApp Gateway API documentation.