---
layout: post
title: Send PDF Files over WhatsApp in Python 3 - Complete Guide
subtitle: Automate WhatsApp document sharing using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2026-02-12T13:15:00+08:00
---

## 🚀 Automate WhatsApp Document Sharing with Python 3

Looking to automate PDF delivery, document notifications, or file sharing from your Python applications? This guide walks you through sending PDF files to WhatsApp users using Python 3 and the WhatsMate WA Gateway REST API. Perfect for Python developers, data scientists, and automation enthusiasts who want to integrate document delivery into their Python-based WhatsApp messaging workflows.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate WA Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Python 3 installed** - Version 3.6+ recommended for modern Python features
4. **PDF file ready** - Have the document you want to send available locally
5. **Requests library** - Install via `pip install requests` if not already available

> ⚠️ **Important**: Recipients must register with the WhatsMate WA Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/whatsapp-gateway-api.html).


### 📝 Step-by-Step Implementation

Follow these steps to send your first PDF document to a WhatsApp user from a Python application:


#### 1. **Copy the Python Code Template**
Start by copying the following source code into your Python file:

<script src="https://gist.github.com/whatsmate/dd8a28d584bc9e8155f42b85e837702a.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the Python code:

- **Lines 8-10**: Replace `YOUR_GATEWAY_INSTANCE_ID_HERE`, `YOUR_OWN_ID_HERE`, and `YOUR_OWN_SECRET_HERE` with your WhatsApp gateway instance ID, Client ID, and Secret
- **Line 14**: Replace `12025550108` with the target phone number (including the country code)
- **Line 15**: Replace `../assets/subwaymap.pdf` with the path to your PDF file
- **Line 16**: Replace `anyname.pdf` with the desired filename for the document
- **Line 17**: Replace `You will find it useful.` with an optional caption for your PDF


#### 3. **Install Required Library**
Ensure you have the `requests` library installed:
```bash
pip install requests
```


#### 4. **Send Your PDF Document**
Run the Python script to deliver your PDF to WhatsApp:
```bash
python3 send-pdf-individual.py
```


### 🔧 Common Use Cases

This automation approach is ideal for:
- **Automated report delivery** - Send daily/weekly PDF reports to WhatsApp from Python applications
- **Document sharing automation** - Deliver invoices, receipts, or contracts via WhatsApp using Python
- **System documentation** - Share configuration files or logs as PDF documents from Python systems
- **Educational content** - Distribute learning materials or tutorials through WhatsApp from Python scripts
- **Integration with Python document generation** - Combine with Python libraries that create PDFs for WhatsApp delivery


### 🚀 Get Started Today

Ready to automate your document sharing over WhatsApp with Python? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/whatsapp-gateway-api.html) and start sending PDF files within minutes!

---

**Next Steps**: Once you've mastered basic PDF sending, explore advanced features like sending [images](https://www.whatsmate.net/whatsapp-image-individual-api.html) or [group messages](https://www.whatsmate.net/whatsapp-group-message-api.html) through the WhatsMate WA Gateway API documentation.