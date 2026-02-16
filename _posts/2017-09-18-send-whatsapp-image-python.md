---
layout: post
title: Send Images over WhatsApp in Python 2 - Legacy Guide
subtitle: Automate WhatsApp image sharing using the WhatsMate WA Gateway REST API (Python 2)
published: true
last_modified_at: 2026-02-11T15:54:00+08:00
---

## ⚠️ Python 2 is Deprecated - Use Python 3 Instead

**Important Note**: Python 2 reached end-of-life on January 1, 2020, and is no longer maintained. This guide is provided for legacy systems only. For new projects, we strongly recommend using our **[Python 3 version](/2020-02-20-send-whatsapp-image-python3/)** which includes modern Python practices and ongoing support.

## Automate WhatsApp Image Sharing with Python 2 (Legacy)

This legacy guide walks you through sending images to WhatsApp users using Python 2 and the WhatsMate WA Gateway REST API. Only use this guide if you're maintaining legacy Python 2 systems. For all new development, use Python 3.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate WA Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Python 2.7 installed** - Legacy Python version (end-of-life)
4. **Image file ready** - Have the image you want to send available locally
5. **Required Python packages** - Install `requests` library: `pip install requests`

> ⚠️ **Important**: Recipients must register with the WhatsMate WA Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/whatsapp-gateway-api.html).


### 📝 Step-by-Step Implementation

Follow these steps to send your first image to a WhatsApp user from a Python 2 application:


#### 1. **Install Required Package**
Ensure you have the `requests` library installed:
```bash
pip install requests
```


#### 2. **Copy the Python 2 Code Template**
Start by copying the following legacy Python 2 source code into your Python file:

<script src="https://gist.github.com/whatsmate/aa79cbc9bded30557f64daefd30f7b2f.js"></script>


#### 3. **Configure a few Parameters**
Customize these key parameters in the Python 2 code:

- **Line 8**: Replace `YOUR_GATEWAY_INSTANCE_ID_HERE` with your WhatsApp gateway instance ID
- **Lines 9-10**: Update `YOUR_OWN_ID_HERE` and `YOUR_OWN_SECRET_HERE` with your Client ID and Secret
- **Line 12**: Replace `12025550108` with the target phone number (including the country code)
- **Line 13**: Replace `../assets/cute-girl.jpg` with the path to your image file
- **Line 14**: Replace `Lovely Gal` with an optional caption for your image


#### 4. **Run Your Python 2 Script**
Execute your Python 2 script to deliver your image to WhatsApp:
```bash
# Navigate to the script directory
cd python

# Make the script executable (Linux/macOS)
chmod +x send-image-individual.py

# Run the script
./send-image-individual.py

# Or run with Python directly
python send-image-individual.py
```


> ⚠️ **Security Warning**: Python 2 no longer receives security updates. Using it in production exposes your system to unpatched vulnerabilities.


### 🚀 Upgrade to Python 3 Today

Ready to modernize your WhatsApp image sharing? Upgrade to our **[Python 3 version](/2020-02-20-send-whatsapp-image-python3/)** which offers:

- **Modern Python 3.6+ support** - Current, maintained Python version
- **Better security** - Regular security updates and patches
- **Improved performance** - Python 3 optimizations and features
- **Future compatibility** - Compatibility with modern libraries and tools
- **Active community support** - Access to current Python ecosystem

[Sign up for a 2-week trial](https://www.whatsmate.net/whatsapp-gateway-api.html) and start sending images with modern Python 3!

---

**Next Steps**: Once you've migrated to Python 3, explore advanced features like sending [documents](https://www.whatsmate.net/whatsapp-document-individual-api.html) or [group messages](https://www.whatsmate.net/whatsapp-group-message-api.html) through the WhatsMate WA Gateway API documentation.