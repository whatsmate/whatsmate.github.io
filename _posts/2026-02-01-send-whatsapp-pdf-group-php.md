---
layout: post
title: Send PDF Files to WhatsApp Groups from PHP - Complete Guide
subtitle: Automate WhatsApp group document sharing using the WhatsMate WA Gateway REST API
redirect_from:
  - /2018-01-20-send-whatsapp-pdf-group-php/
published: true
last_modified_at: 2026-03-12T11:05:09+08:00
---

## Automate WhatsApp Group Document Sharing with PHP

Need to integrate WhatsApp group PDF sharing into your PHP applications for report distribution, automated documentation delivery, or website file sharing? This guide shows you how to deliver PDF files to WhatsApp groups using PHP and the WhatsMate WA Gateway REST API. Perfect for PHP developers building websites, web applications, or any PHP-based system that needs document delivery to group chats.

### Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate WA Gateway Forever Green account** - Required for group messaging API access
2. **Group setup** - Create a WhatsApp group with a unique name and add the gateway
3. **PHP installed** - Version 7.0 or higher with cURL extension enabled
4. **Web server** - Apache, Nginx, or any server that can execute PHP
5. **PDF file ready** - Have the document you want to send available on your server

> ⚠️ **Important**: You need a Forever Green account to send messages to WhatsApp groups. The gateway must be added to your WhatsApp group before it can send messages. [Sign up for a Forever Green account](https://www.whatsmate.net/whatsapp-group-message-api.html) to enable group messaging capabilities.

> **Document Requirements**: The script supports PDF files and other document types (MP4, WAV, etc.). Ensure your file is accessible and not corrupted before sending.

### Step-by-Step Implementation

Follow these steps to send your first PDF document to a WhatsApp group from a PHP application:

#### 1. **Prepare Your WhatsApp Group**
Before coding, set up your WhatsApp group:

1. Create a new group in WhatsApp with a **unique name** (the API won't work if the name isn't unique)
2. Add the secret gateway number to the group
3. Send a "Hi" message (or any message) in the group from your personal WhatsApp account - this helps the gateway silently recognize the new group in the background

#### 2. **Copy the PHP Source Code**
Start by copying the following source code into your PHP script:

{% include gist-styles.html %}

<script src="https://gist.github.com/whatsmate/cb12ec0a92f623f06069ee9a43d5bac2.js"></script>

#### 3. **Configure Key Parameters**
Customize these essential parameters in the PHP script:

- **Lines 2-4**: Replace `YOUR_INSTANCE_ID_HERE`, `YOUR_CLIENT_ID_HERE`, and `YOUR_CLIENT_SECRET_HERE` with your Forever Green credentials
- **Line 6**: Replace `/tmp/your_doc.pdf` with the path to your PDF file on the server
- **Line 9**: Replace `anyname.pdf` with the desired filename for the document
- **Line 10**: Replace `"You will find the map handy."` with an optional caption for your PDF
- **Line 13**: Specify your group name (must be unique)

#### 4. **Upload and Execute**
1. Save the PHP file to your web server (e.g., `send-pdf-group.php`)
2. Ensure the PDF file is accessible at the path specified in line 6 and that PHP has read permissions
3. Visit the PHP page in your browser or execute via command line to send your PDF

**To execute via command line:**
```bash
php send-pdf-group.php
```

**To execute via web browser:**
Simply navigate to `http://your-domain.com/send-pdf-group.php`

### Common Use Cases

This PHP integration is ideal for:
- **Website document distribution** - Allow users to download PDFs that get shared to WhatsApp groups automatically
- **E-commerce order confirmations** - Automatically send invoices or receipts to customer WhatsApp groups
- **Content management systems** - Integrate with WordPress, Joomla, or Drupal to share documents to groups
- **Web application reporting** - Generate and deliver PDF reports from PHP web apps to team WhatsApp groups
- **Automated documentation delivery** - Send system logs or documentation as PDFs to admin groups

### Get Started Today

Ready to integrate WhatsApp group PDF sharing into your PHP applications? You'll need a Forever Green account to access the group messaging API. [Sign up for a Forever Green account](https://www.whatsmate.net/whatsapp-group-message-api.html) and start sending PDF documents to groups within minutes!

---

**Next Steps**: Once you've mastered group PDF sending, explore advanced features like sending [images to groups](https://www.whatsmate.net/whatsapp-group-image-api.html) or [individual messages](https://www.whatsmate.net/whatsapp-gateway-api.html) through the WhatsMate WA Gateway API documentation.
