---
layout: post
title: Send PDF Files to WhatsApp Groups in Node.js - Complete Guide
subtitle: Automate WhatsApp group document sharing using the WhatsMate WA Gateway REST API
redirect_from:
  - /2018-01-22-send-whatsapp-pdf-group-nodejs-javascript/
published: true
last_modified_at: 2026-03-12T11:05:09+08:00
---

## Automate WhatsApp Group Document Sharing with Node.js

Need to integrate WhatsApp group PDF sharing into your Node.js applications for report distribution, automated documentation delivery, or backend file sharing? This guide shows you how to deliver PDF files to WhatsApp groups using Node.js and the WhatsMate WA Gateway REST API. Perfect for JavaScript/Node.js developers building web applications, backend services, or any Node.js-based system that needs document delivery to group chats.

### Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate WA Gateway Forever Green account** - Required for group messaging API access
2. **Group setup** - Create a WhatsApp group with a unique name and add the gateway
3. **Node.js installed** - Version 12 or higher recommended
4. **Basic JavaScript/Node.js knowledge** - Familiarity with Node.js modules and file system operations
5. **PDF file ready** - Have the document you want to send available locally

> ⚠️ **Important**: You need a Forever Green account to send messages to WhatsApp groups. The gateway must be added to your WhatsApp group before it can send messages. [Sign up for a Forever Green account](https://www.whatsmate.net/whatsapp-group-message-api.html) to enable group messaging capabilities.

> **Document Requirements**: The script supports PDF files and other document types (MP4, WAV, etc.). Ensure your file is accessible and not corrupted before sending.

### Step-by-Step Implementation

Follow these steps to send your first PDF document to a WhatsApp group from a Node.js application:

#### 1. **Prepare Your WhatsApp Group**
Before coding, set up your WhatsApp group:

1. Create a new group in WhatsApp with a **unique name** (the API won't work if the name isn't unique)
2. Add the secret gateway number to the group
3. Send a "Hi" message (or any message) in the group from your personal WhatsApp account - this helps the gateway silently recognize the new group in the background

#### 2. **Copy the Node.js Source Code**
Start by copying the following source code into your Node.js script:

{% include gist-styles.html %}

<script src="https://gist.github.com/whatsmate/cbf97a5b5b9da750222f8061a2a19141.js"></script>

#### 3. **Configure Key Parameters**
Customize these essential parameters in the Node.js script:

- **Lines 7-9**: Replace `YOUR_OWN_GATEWAY_INSTANCE_ID`, `YOUR_OWN_CLIENT_ID`, and `YOUR_OWN_SECRET_ID` with your Forever Green credentials
- **Line 12**: Specify your group name (must be unique)
- **Line 13**: Replace `"../assets/subwaymap.pdf"` with the path to your PDF file
- **Line 14**: Replace `"anyname.pdf"` with the desired filename for the document
- **Line 15**: Replace `"Hope you like it"` with an optional caption for your PDF

#### 4. **Make the Script Executable**
Set execute permissions on your Node.js script:
```bash
chmod 755 send-pdf-group.js
```

#### 5. **Send Your PDF Document**
Run the script to deliver your PDF to the WhatsApp group:
```bash
./send-pdf-group.js
```

**Alternative execution method (without making executable):**
```bash
node send-pdf-group.js
```

### Common Use Cases

This Node.js integration is ideal for:
- **Real-time web applications** - Send PDF reports or documents from Express.js, Socket.io, or real-time dashboards to WhatsApp groups
- **Backend microservices** - Integrate WhatsApp PDF sharing into Node.js microservices, APIs, or serverless functions
- **Automation workflows** - Trigger document delivery from CI/CD pipelines, monitoring systems, or scheduled Node.js tasks
- **Full-stack JavaScript applications** - Send group documents from React, Vue, or Angular applications with Node.js backends
- **Batch document processing** - Integrate PDF delivery into larger Node.js data processing workflows

### Get Started Today

Ready to integrate WhatsApp group PDF sharing into your Node.js applications? You'll need a Forever Green account to access the group messaging API. [Sign up for a Forever Green account](https://www.whatsmate.net/whatsapp-group-message-api.html) and start sending PDF documents to groups within minutes!

---

**Next Steps**: Once you've mastered group PDF sending, explore advanced features like sending [images to groups](https://www.whatsmate.net/whatsapp-group-image-api.html) or [individual messages](https://www.whatsmate.net/whatsapp-gateway-api.html) through the WhatsMate WA Gateway API documentation.
