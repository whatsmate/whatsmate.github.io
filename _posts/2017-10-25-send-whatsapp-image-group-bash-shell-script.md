---
layout: post
title: Send Images to WhatsApp Groups from Shell Script - Complete Guide
subtitle: Automate WhatsApp group image sharing using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2026-02-13T14:30:00+08:00
---

## Automate WhatsApp Group Image Sharing with Shell Scripts

Need to send images to WhatsApp groups for team updates, visual reports, or automated notifications? This guide shows you how to deliver images to WhatsApp groups using a simple shell script and the WhatsMate WA Gateway REST API. Ideal for team leaders, system administrators, and developers who want to automate visual content delivery to group chats.

### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate WA Gateway Forever Green account** - Required for group messaging API access
2. **Group setup** - Create a WhatsApp group with a unique name and add the gateway
3. **Unix/Linux system with curl and base64** - Shell script requires bash, curl, and base64 commands
4. **Image file ready** - Have the image you want to send available locally

> ⚠️ **Important**: You need a Forever Green account to send messages to WhatsApp groups. The gateway must be added to your WhatsApp group before it can send messages. [Sign up for a Forever Green account](https://www.whatsmate.net/whatsapp-group-message-api.html) to enable group messaging capabilities.

### 📝 Step-by-Step Implementation

Follow these steps to send your first image to a WhatsApp group from a shell script:

#### 1. **Prepare Your WhatsApp Group**
Before coding, set up your WhatsApp group:

1. Create a new group in WhatsApp with a **unique name** (the API won't work if the name isn't unique)
2. Add the secret gateway number to the group
3. Send a "Hi" message (or any message) in the group from your personal WhatsApp account - this helps the gateway silently recognize the new group in the background

#### 2. **Copy the Script Template**
Start by copying the following source code into your script file:

<script src="https://gist.github.com/whatsmate/3392b82db3187565d19097bd5c22bfd2.js"></script>

#### 3. **Configure Key Parameters**
Customize these essential parameters in the shell script:

- **Line 13**: Replace `YOUR_OWN_INSTANCE_ID_HERE` with your WhatsApp gateway instance ID
- **Lines 14-15**: Update `YOUR_OWN_CLIENT_ID_HERE` and `YOUR_OWN_SECRET_HERE` with your Forever Green Client ID and Secret
- **Line 18**: Specify your group name (must be unique)
- **Line 19**: Replace `../assets/cute-girl.jpg` with the path to your image file
- **Line 24**: Replace `"Lovely Gal"` with an optional caption for your image

> 💡 **Note**: The script uses the `base64` utility to encode your image. If it's not available on your system, install it with `sudo apt-get install coreutils` (Debian/Ubuntu) or equivalent for your distribution.

#### 4. **Make the Script Executable**
Set execute permissions on your script:
```bash
chmod 755 send-image-group.sh
```

#### 5. **Send Your Image**
Run the script to deliver your image to the WhatsApp group:
```bash
./send-image-group.sh
```

### 🔧 Common Use Cases

This automation approach is ideal for:
- **Team visual updates** - Send project screenshots or progress images to team WhatsApp groups
- **Automated group notifications** - Deliver visual alerts or status images to group members
- **Group photo sharing** - Automatically share daily photos or visual content with WhatsApp groups
- **Visual reporting** - Send charts, graphs, or diagrams to group chats for collaborative review
- **Integration with monitoring systems** - Combine with scripts that generate system status images for group notifications

### 🚀 Get Started Today

Ready to automate image sharing to WhatsApp groups? You'll need a Forever Green account to access the group messaging API. [Sign up for a Forever Green account](https://www.whatsmate.net/whatsapp-group-message-api.html) and start sending images to groups within minutes!

---

**Next Steps**: Once you've mastered group image sending, explore advanced features like sending [documents to groups](https://www.whatsmate.net/whatsapp-group-document-api.html) or [individual messages](https://www.whatsmate.net/whatsapp-gateway-api.html) through the WhatsMate WA Gateway API documentation.