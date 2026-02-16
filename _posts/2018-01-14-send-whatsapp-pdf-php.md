---
layout: post
title: Send PDF Files over WhatsApp in PHP - Complete Guide
subtitle: Automate WhatsApp document sharing using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2026-02-12T13:00:00+08:00
---

## Automate WhatsApp Document Sharing with PHP

Looking to automate PDF delivery, document notifications, or file sharing from your PHP applications? This guide walks you through sending PDF files to WhatsApp users using PHP and the WhatsMate WA Gateway REST API. Perfect for PHP developers, web administrators, and automation enthusiasts who want to integrate document delivery into their PHP-based WhatsApp messaging workflows.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate WA Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **PHP development environment** - PHP installed and configured (version 5.4 or higher)
4. **Web server access** - Ability to run PHP scripts on a web server
5. **PDF file ready** - Have the document you want to send available on your server

> ⚠️ **Important**: Recipients must register with the WhatsMate WA Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/whatsapp-gateway-api.html).


### 📝 Step-by-Step Implementation

Follow these steps to send your first PDF document to a WhatsApp user from a PHP script:


#### 1. **Copy the PHP Code Template**
Start by copying the following source code into your PHP file:

<script src="https://gist.github.com/whatsmate/188993db93efa86b979df6aabf903d53.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the PHP code:

- **Lines 2-4**: Replace `YOUR_INSTANCE_ID_HERE`, `YOUR_CLIENT_ID_HERE`, and `YOUR_CLIENT_SECRET_HERE` with your WhatsApp gateway instance ID, Client ID, and Secret
- **Line 6**: Replace `/tmp/your_doc.pdf` with the path to your PDF file
- **Line 9**: Replace `anyname.pdf` with the desired filename for the document
- **Line 10**: Replace `You will find the map handy.` with an optional caption for your PDF
- **Line 13**: Replace `12025550108` with the target phone number (including the country code)


#### 3. **Upload to Your Web Server**
Upload the PHP file to your web server where PHP is enabled and configured.


#### 4. **Send Your PDF Document**
Access the PHP script through your web browser to deliver your PDF to WhatsApp.


### 🔧 Common Use Cases

This automation approach is ideal for:
- **Automated report delivery** - Send daily/weekly PDF reports to WhatsApp from PHP web applications
- **Document sharing automation** - Deliver invoices, receipts, or contracts via WhatsApp using PHP
- **System documentation** - Share configuration files or logs as PDF documents from PHP systems
- **Educational content** - Distribute learning materials or tutorials through WhatsApp from PHP sites
- **Integration with PHP document generation** - Combine with PHP libraries that create PDFs for WhatsApp delivery


### 🚀 Get Started Today

Ready to automate your document sharing over WhatsApp with PHP? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/whatsapp-gateway-api.html) and start sending PDF files within minutes!

---

**Next Steps**: Once you've mastered basic PDF sending, explore advanced features like sending [images](https://www.whatsmate.net/whatsapp-image-individual-api.html) or [group messages](https://www.whatsmate.net/whatsapp-group-message-api.html) through the WhatsMate WA Gateway API documentation.