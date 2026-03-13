---
layout: post
title: Send PDF Files to WhatsApp Groups from Shell Script - Complete Guide
subtitle: Automate WhatsApp group document sharing using the WhatsMate WA Gateway REST API
redirect_from:
  - /2018-01-18-send-whatsapp-pdf-group-bash-shell-script/
published: true
last_modified_at: 2026-03-12T11:05:09+08:00
---

## Automate WhatsApp Group Document Sharing with Shell Scripts

Need to send PDF documents to WhatsApp groups for team reports, automated documentation delivery, or file distribution? This guide shows you how to deliver PDF files to WhatsApp groups using a simple shell script and the WhatsMate WA Gateway REST API. Perfect for team leaders, system administrators, and developers who want to automate document delivery to group chats directly from the terminal.

### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate WA Gateway Forever Green account** - Required for group messaging API access
2. **Group setup** - Create a WhatsApp group with a unique name and add the gateway
3. **Unix/Linux system with curl and base64** - Shell script requires bash, curl, and base64 commands
4. **PDF file ready** - Have the document you want to send available locally

> ⚠️ **Important**: You need a Forever Green account to send messages to WhatsApp groups. The gateway must be added to your WhatsApp group before it can send messages. [Sign up for a Forever Green account](https://www.whatsmate.net/whatsapp-group-message-api.html) to enable group messaging capabilities.

> 📄 **Document Requirements**: The script supports PDF files and other document types (MP4, WAV, etc.). Ensure your file is accessible and not corrupted before sending.

### 📝 Step-by-Step Implementation

Follow these steps to send your first PDF document to a WhatsApp group from a shell script:

#### 1. **Prepare Your WhatsApp Group**
Before coding, set up your WhatsApp group:

1. Create a new group in WhatsApp with a **unique name** (the API won't work if the name isn't unique)
2. Add the secret gateway number to the group
3. Send a "Hi" message (or any message) in the group from your personal WhatsApp account - this helps the gateway silently recognize the new group in the background

#### 2. **Copy the Script Template**
Start by copying the following source code into your script file:

<script src="https://gist.github.com/whatsmate/d58030fa593d0f7893a5807a056a310a.js"></script>

#### 3. **Configure Key Parameters**
Customize these essential parameters in the shell script:

- **Line 11-12**: Replace `YOUR_OWN_CLIENT_ID_HERE` and `YOUR_OWN_SECRET_HERE` with your Forever Green Client ID and Secret
- **Line 15**: Specify your group name (must be unique)
- **Line 16**: Replace `../assets/subwaymap.pdf` with the path to your PDF file
- **Line 17**: Replace `map.pdf` with the desired filename for the document
- **Line 18**: Replace `"You will find it handy."` with an optional caption for your PDF

> 💡 **Note**: The script uses the `base64` utility to encode your PDF document. If it's not available on your system, install it with `sudo apt-get install coreutils` (Debian/Ubuntu) or equivalent for your distribution.

#### 4. **Install Base64 Utility (If Needed)**
Ensure the `base64` command is available on your system:
```bash
# For Debian/Ubuntu systems:
sudo apt-get install coreutils

# For RHEL/CentOS systems:
sudo yum install coreutils
```

#### 5. **Make the Script Executable**
Set execute permissions on your script:
```bash
chmod 755 send-pdf-group.sh
```

#### 6. **Send Your PDF Document**
Run the script to deliver your PDF to the WhatsApp group:
```bash
./send-pdf-group.sh
```

### 🔧 Common Use Cases

This automation approach is ideal for:
- **Team document sharing** - Send reports, manuals, or guidelines to team WhatsApp groups
- **Automated report distribution** - Deliver generated PDF reports to group members automatically
- **Document collaboration** - Share working documents or drafts with project groups via WhatsApp
- **System documentation delivery** - Automatically send system logs or documentation as PDFs to admin groups
- **Integration with document generation** - Combine with scripts that create PDFs for automated delivery to groups

### 🚀 Get Started Today

Ready to automate PDF sharing to WhatsApp groups? You'll need a Forever Green account to access the group messaging API. [Sign up for a Forever Green account](https://www.whatsmate.net/whatsapp-group-message-api.html) and start sending PDF documents to groups within minutes!

---

**Next Steps**: Once you've mastered group PDF sending, explore advanced features like sending [images to groups](https://www.whatsmate.net/whatsapp-group-image-api.html) or [individual messages](https://www.whatsmate.net/whatsapp-gateway-api.html) through the WhatsMate WA Gateway API documentation.
