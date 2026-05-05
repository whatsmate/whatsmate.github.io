---
layout: post
title: Send PDF Files to WhatsApp Groups in Python 3 - Complete Guide
subtitle: Automate WhatsApp group document sharing using the WhatsMate WA Gateway REST API
redirect_from:
  - /2020-02-23-send-whatsapp-pdf-group-python3/
published: true
last_modified_at: 2026-03-12T11:05:09+08:00
---

## Automate WhatsApp Group Document Sharing with Python 3

Need to integrate WhatsApp group PDF sharing into your Python applications for report distribution, automated documentation delivery, or data pipeline file sharing? This guide shows you how to deliver PDF files to WhatsApp groups using Python 3 and the WhatsMate WA Gateway REST API. Perfect for Python developers building automation scripts, data science workflows, web applications, or any Python project that needs document delivery to group chats.

### Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate WA Gateway Forever Green account** - Required for group messaging API access
2. **Group setup** - Create a WhatsApp group with a unique name and add the gateway
3. **Python 3 installed** - Version 3.6 or higher with pip package manager
4. **Required Python packages** - `requests` library (installation instructions included)
5. **PDF file ready** - Have the document you want to send available locally

> ⚠️ **Important**: You need a Forever Green account to send messages to WhatsApp groups. The gateway must be added to your WhatsApp group before it can send messages. [Sign up for a Forever Green account](https://www.whatsmate.net/whatsapp-group-message-api.html) to enable group messaging capabilities.

> **Document Requirements**: The script supports PDF files and other document types (MP4, WAV, etc.). Ensure your file is accessible and not corrupted before sending.

### Step-by-Step Implementation

Follow these steps to send your first PDF document to a WhatsApp group from a Python script:

#### 1. **Prepare Your WhatsApp Group**
Before coding, set up your WhatsApp group:

1. Create a new group in WhatsApp with a **unique name** (the API won't work if the name isn't unique)
2. Add the secret gateway number to the group
3. Send a "Hi" message (or any message) in the group from your personal WhatsApp account - this helps the gateway silently recognize the new group in the background

#### 2. **Install Required Package**
Install the `requests` library if you don't have it already:
```bash
pip install requests
```

#### 3. **Copy the Python Source Code**
Start by copying the following source code into your Python script:

{% include gist-styles.html %}

<script src="https://gist.github.com/whatsmate/f0a51f7569a8c007f66c88ed419d3406.js"></script>

#### 4. **Configure Key Parameters**
Customize these essential parameters in the Python code:

- **Lines 8-10**: Replace `YOUR_GATEWAY_INSTANCE_ID_HERE`, `YOUR_OWN_ID_HERE`, and `YOUR_OWN_SECRET_HERE` with your Forever Green credentials
- **Line 13**: Specify your group name (must be unique)
- **Line 14**: Replace `../assets/subwaymap.pdf` with the path to your PDF file
- **Line 15**: Replace `anyname.pdf` with the desired filename for the document
- **Line 16**: Replace `"You will find it useful."` with an optional caption for your PDF

#### 5. **Make the Script Executable**
Set execute permissions on your Python script:
```bash
chmod 755 send-pdf-group.py
```

#### 6. **Send Your PDF Document**
Run the script to deliver your PDF to the WhatsApp group:
```bash
./send-pdf-group.py
```

**Alternative execution method (without making executable):**
```bash
python3 send-pdf-group.py
```

### Common Use Cases

This Python 3 integration is ideal for:
- **Data science workflows** - Send PDF reports or analysis results to team WhatsApp groups
- **Automation scripts** - Create scheduled tasks that send daily reports or documentation to groups
- **Web application backends** - Integrate WhatsApp PDF sharing into Django or Flask applications
- **Monitoring systems** - Automatically send system logs or documentation as PDFs to admin groups
- **Batch document processing** - Integrate PDF delivery into larger Python data processing workflows

### Get Started Today

Ready to automate WhatsApp group PDF sharing with Python 3? You'll need a Forever Green account to access the group messaging API. [Sign up for a Forever Green account](https://www.whatsmate.net/whatsapp-group-message-api.html) and start sending PDF documents to groups within minutes!

---

**Next Steps**: Once you've mastered group PDF sending, explore advanced features like sending [images to groups](https://www.whatsmate.net/whatsapp-group-image-api.html) or [individual messages](https://www.whatsmate.net/whatsapp-gateway-api.html) through the WhatsMate WA Gateway API documentation.
