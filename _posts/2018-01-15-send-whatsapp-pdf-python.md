---
layout: post
title: Send PDF Files over WhatsApp in Python 2 - Complete Guide
subtitle: Automate WhatsApp document sharing using the WhatsMate WA Gateway REST API (Legacy Python 2)
published: true
last_modified_at: 2026-02-12T13:30:00+08:00
---

## 🚀 Automate WhatsApp Document Sharing with Python 2 (Legacy)

> ⚠️ **Python 2 Notice**: Python 2 reached end-of-life in January 2020 and is no longer maintained. This guide is provided for legacy systems that still require Python 2 support. For new projects, we strongly recommend using **[Python 3 instead](2020-02-22-send-whatsapp-pdf-python3.md)**.

Looking to automate PDF delivery, document notifications, or file sharing from legacy Python 2 applications? This guide walks you through sending PDF files to WhatsApp users using Python 2 and the WhatsMate WA Gateway REST API. Perfect for maintaining legacy Python 2 systems that need WhatsApp document delivery capabilities.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate WA Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Python 2 installed** - Version 2.7+ (legacy Python 2 environment)
4. **PDF file ready** - Have the document you want to send available locally
5. **Requests library** - Install via `pip install requests` if not already available

> ⚠️ **Important**: Recipients must register with the WhatsMate WA Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/whatsapp-gateway-api.html).


### 📝 Step-by-Step Implementation

Follow these steps to send your first PDF document to a WhatsApp user from a Python 2 application:


#### 1. **Copy the Python 2 Code Template**
Start by copying the following source code into your Python file:

<script src="https://gist.github.com/whatsmate/0cd18f0e4d296d5d56ab310ec20efb20.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the Python 2 code:

- **Lines 8-10**: Replace `YOUR_GATEWAY_INSTANCE_ID_HERE`, `YOUR_OWN_ID_HERE`, and `YOUR_OWN_SECRET_HERE` with your WhatsApp gateway instance ID, Client ID, and Secret
- **Line 13**: Replace `12025550108` with the target phone number (including the country code)
- **Line 14**: Replace `../assets/subwaymap.pdf` with the path to your PDF file
- **Line 15**: Replace `anyname.pdf` with the desired filename for the document
- **Line 16**: Replace `You will find it useful` with an optional caption for your PDF


#### 3. **Install Required Library**
Ensure you have the `requests` library installed for Python 2:
```bash
pip install requests
```

> **Note**: For Python 2 systems, you may need to use `pip2` instead of `pip` depending on your system configuration.


#### 4. **Send Your PDF Document**
Run the Python 2 script to deliver your PDF to WhatsApp:
```bash
python send-pdf-individual.py
```


### 🔧 Common Use Cases

This legacy automation approach is ideal for:
- **Maintaining legacy systems** - Send PDF reports from existing Python 2 applications that cannot be upgraded
- **Document sharing for legacy infrastructure** - Deliver invoices or contracts via WhatsApp from Python 2 systems
- **Legacy system documentation** - Share configuration files or logs as PDF documents from Python 2 environments
- **Educational content for legacy platforms** - Distribute materials through WhatsApp from Python 2 scripts
- **Integration with legacy document generation** - Combine with Python 2 libraries that create PDFs for WhatsApp delivery


### 🚀 Get Started Today

Ready to automate your document sharing over WhatsApp with Python 2? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/whatsapp-gateway-api.html) and start sending PDF files within minutes!

---

**Next Steps**: 
- **For new projects**: Use **[Python 3 instead](2020-02-22-send-whatsapp-pdf-python3.md)** for modern Python development with ongoing support
- **Explore advanced features**: Once you've mastered basic PDF sending, explore sending [images](https://www.whatsmate.net/whatsapp-image-individual-api.html) or [group messages](https://www.whatsmate.net/whatsapp-group-message-api.html) through the WhatsMate WA Gateway API documentation.