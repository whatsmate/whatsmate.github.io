---
layout: post
title: Send PDF Files to Telegram Groups from Shell Script - Complete Guide
subtitle: Automate Telegram group document sharing using the WhatsMate Telegram Gateway REST API
published: true
last_modified_at: 2026-02-06T20:30:00+08:00
---

## Automate Telegram Group Document Sharing with Shell Scripts

Need to send PDF documents to Telegram groups for team collaboration, report distribution, or automated documentation delivery? This guide shows you how to deliver PDF files to Telegram groups using a simple shell script and the WhatsMate Telegram Gateway REST API. Perfect for team leaders, system administrators, and developers who want to automate document delivery to group chats directly from the terminal.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate Telegram Gateway account** - Required for API access
2. **Group membership** - The gateway must be a member of the target Telegram group
3. **Basic shell scripting knowledge** - Familiarity with terminal commands
4. **PDF file ready** - Have the document you want to send available locally
5. **Base64 utility** - The `base64` command must be available on your system

> ⚠️ **Important**: The gateway must be a member of the Telegram group you want to send messages to. The group admin phone number is used to uniquely identify the group.

> 📄 **Document Requirements**: The script supports PDF files and other document types. Ensure your file is accessible and not corrupted before sending.


### 🎥 Video Walkthrough

<iframe width="560" height="315" src="https://www.youtube.com/embed/5O3ZpZ1CfzI?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


### 📝 Step-by-Step Implementation

Follow these steps to send your first PDF document to a Telegram group from a shell script:


#### 1. **Copy the Script Template**
Start by copying the following source code into your script file:

<script src="https://gist.github.com/whatsmate/3d863e5beca363d71ecf205401dd5322.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the script:

- **Line 13**: Replace `YOUR_OWN_INSTANCE_ID_HERE` with your Telegram gateway instance ID
- **Lines 14-15**: Update `YOUR_OWN_CLIENT_ID_HERE` and `YOUR_OWN_SECRET_HERE` with your Client ID and Secret
- **Line 18**: Replace `"Muscle Men Club"` with the name of your target Telegram group
- **Line 19**: Replace `"12025550108"` with the phone number of the group admin (including country code)
- **Line 20**: Replace `../assets/subwaymap.pdf` with the path to your PDF file
- **Line 21**: Replace `"map.pdf"` with the desired filename for the document
- **Line 22**: Replace `"Check this out"` with an optional caption for your PDF


#### 3. **Install Base64 Utility (If Needed)**
Ensure the `base64` command is available on your system:
```bash
# For Debian/Ubuntu systems:
sudo apt-get install coreutils

# For RHEL/CentOS systems:
sudo yum install coreutils
```


#### 4. **Make the Script Executable**
Set execute permissions on your script:
```bash
chmod 755 group-send-telegram-pdf.sh
```


#### 5. **Send Your PDF Document**
Run the script to deliver your PDF to the Telegram group:
```bash
./group-send-telegram-pdf.sh
```


### 🔧 Common Use Cases

This automation approach is ideal for:
- **Team document sharing** - Send reports, manuals, or guidelines to team Telegram groups
- **Automated report distribution** - Deliver generated PDF reports to group members automatically
- **Document collaboration** - Share working documents or drafts with project groups via Telegram
- **System documentation delivery** - Automatically send system logs or documentation as PDFs to admin groups
- **Integration with document generation** - Combine with scripts that create PDFs for automated delivery to groups


### 🚀 Get Started Today

Ready to automate PDF sharing to Telegram groups? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/telegram-gateway-api.html) and start sending PDF documents to groups within minutes!

---

**Next Steps**: Once you've mastered group PDF sending, explore advanced features like sending [images to groups](https://www.whatsmate.net/telegram-group-image-api.html), [audio files to groups](https://www.whatsmate.net/telegram-group-audio-api.html), or [individual messages](https://www.whatsmate.net/telegram-gateway-api.html) through the WhatsMate Telegram Gateway API documentation.

