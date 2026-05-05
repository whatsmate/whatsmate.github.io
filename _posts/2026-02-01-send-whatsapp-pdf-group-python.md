---
layout: post
title: Send PDF Files to WhatsApp Groups in Python 2 - Legacy Guide
subtitle: Automate WhatsApp group document sharing using the WhatsMate WA Gateway REST API (Python 2)
redirect_from:
  - /2018-01-21-send-whatsapp-pdf-group-python/
published: true
last_modified_at: 2026-03-12T11:05:09+08:00
---

## ⚠️ Python 2 is Deprecated - Use Python 3 Instead

**Important Note**: Python 2 reached end-of-life on January 1, 2020, and is no longer maintained. This guide is provided for legacy systems only. For new projects, we strongly recommend using our **[Python 3 version](/2020-02-23-send-whatsapp-pdf-group-python3/)** which includes modern Python practices and ongoing support.

## Automate WhatsApp Group Document Sharing with Python 2 (Legacy)

Need to integrate WhatsApp group PDF sharing into legacy Python 2 applications for report distribution or automated documentation delivery? This legacy guide shows you how to deliver PDF files to WhatsApp groups using Python 2 and the WhatsMate WA Gateway REST API. Only use this guide if you're maintaining legacy Python 2 systems. For all new development, use Python 3.

### Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate WA Gateway Forever Green account** - Required for group messaging API access
2. **Group setup** - Create a WhatsApp group with a unique name and add the gateway
3. **Python 2.7 installed** - Legacy Python version (end-of-life)
4. **Required Python packages** - `requests` library (installation instructions included)
5. **PDF file ready** - Have the document you want to send available locally

> ⚠️ **Important**: You need a Forever Green account to send messages to WhatsApp groups. The gateway must be added to your WhatsApp group before it can send messages. [Sign up for a Forever Green account](https://www.whatsmate.net/whatsapp-group-message-api.html) to enable group messaging capabilities.

> **Document Requirements**: The script supports PDF files and other document types (MP4, WAV, etc.). Ensure your file is accessible and not corrupted before sending.

### Step-by-Step Implementation

Follow these steps to send your first PDF document to a WhatsApp group from a legacy Python 2 script:

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

#### 3. **Copy the Python 2 Source Code**
Start by copying the following legacy Python 2 source code into your script:

{% include gist-styles.html %}

<script src="https://gist.github.com/whatsmate/c402e9b7494f90e6a490bbf4643393a6.js"></script>

#### 4. **Configure Key Parameters**
Customize these essential parameters in the Python 2 code:

- **Lines 8-10**: Replace `YOUR_GATEWAY_INSTANCE_ID_HERE`, `YOUR_OWN_ID_HERE`, and `YOUR_OWN_SECRET_HERE` with your Forever Green credentials
- **Line 13**: Specify your group name (must be unique)
- **Line 14**: Replace `../assets/subwaymap.pdf` with the path to your PDF file
- **Line 15**: Replace `anyname.pdf` with the desired filename for the document
- **Line 16**: Replace `"You will find it useful"` with an optional caption for your PDF

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
python send-pdf-group.py
```

### Common Use Cases (Legacy Systems)

This Python 2 integration is for legacy systems only and is ideal for:
- **Legacy enterprise applications** - Maintain WhatsApp group PDF sharing in existing Python 2 business systems
- **Older automation scripts** - Support scheduled tasks sending reports in legacy Python 2 environments
- **System migration projects** - Maintain functionality during transition from Python 2 to Python 3
- **Legacy monitoring tools** - Integrate with older system monitoring applications that generate PDF logs
- **Historical codebases** - Support maintenance of Python 2 code that cannot be immediately upgraded

### Get Started Today (For Legacy Systems Only)

Ready to maintain WhatsApp group PDF sharing in your legacy Python 2 applications? You'll need a Forever Green account to access the group messaging API. [Sign up for a Forever Green account](https://www.whatsmate.net/whatsapp-group-message-api.html) to enable group messaging capabilities.

**⚠️ Important Reminder**: Python 2 is no longer supported. Consider migrating to **[Python 3](/2020-02-23-send-whatsapp-pdf-group-python3/)** for security updates, new features, and ongoing community support.

---

**Next Steps**: Once you've mastered group PDF sending, explore advanced features like sending [images to groups](https://www.whatsmate.net/whatsapp-group-image-api.html) or [individual messages](https://www.whatsmate.net/whatsapp-gateway-api.html) through the WhatsMate WA Gateway API documentation.

**Migration Recommendation**: For long-term maintainability and security, plan your migration to Python 3 using our [Python 3 WhatsApp group PDF sending guide](/2020-02-23-send-whatsapp-pdf-group-python3/).
