---
layout: post
title: Send Images over WhatsApp in Node.js/JavaScript - Complete Guide
subtitle: Automate WhatsApp image sharing using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2026-02-11T15:54:00+08:00
---

## Automate WhatsApp Image Sharing with Node.js/JavaScript

Looking to automate WhatsApp image sharing, visual notifications, or media delivery from your JavaScript applications? This guide walks you through sending images to WhatsApp users using Node.js and the WhatsMate WA Gateway REST API. Perfect for JavaScript developers, full-stack engineers, and Node.js enthusiasts who want to integrate visual content delivery into their JavaScript-based workflows.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate WA Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Node.js installed** - Version 12+ recommended for modern JavaScript features
4. **Image file ready** - Have the image you want to send available locally

> ⚠️ **Important**: Recipients must register with the WhatsMate WA Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/whatsapp-gateway-api.html).


### 📝 Step-by-Step Implementation

Follow these steps to send your first image to a WhatsApp user from a Node.js application:


#### 1. **Copy the Node.js Code Template**
Start by copying the following source code into your JavaScript file:

<script src="https://gist.github.com/whatsmate/a4a98f7d863640922ca2c32f91bcf364.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the JavaScript code:

- **Line 7**: Replace `YOUR_OWN_GATEWAY_INSTANCE_ID` with your WhatsApp gateway instance ID
- **Lines 8-9**: Update `YOUR_OWN_CLIENT_ID` and `YOUR_OWN_SECRET_ID` with your Client ID and Secret
- **Line 12**: Replace `12025550108` with the target phone number (including the country code)
- **Line 13**: Replace `../assets/cute-girl.jpg` with the path to your image file
- **Line 14**: Replace `Lovely Gal` with an optional caption for your image


#### 3. **Run Your Node.js Script**
Execute your JavaScript script to deliver your image to WhatsApp:
```bash
# Navigate to the script directory
cd nodejs

# Make the script executable (Linux/macOS)
chmod +x send-image-individual.js

# Run the script directly (requires shebang line)
./send-image-individual.js

# Or run with Node.js directly
node send-image-individual.js
```


### 🔧 Common Use Cases

This automation approach is ideal for:
- **Full-stack applications** - Send images to WhatsApp from Express.js, Nest.js, or other Node.js frameworks
- **Serverless functions** - Integrate WhatsApp image sharing into AWS Lambda, Azure Functions, or Google Cloud Functions
- **Microservices** - Add WhatsApp notifications with images to Node.js microservices
- **Automation scripts** - Use Node.js for scheduled image delivery and automation workflows
- **Real-time applications** - Deliver images via WhatsApp from Socket.io or WebSocket applications


### 🚀 Get Started Today

Ready to automate your image sharing over WhatsApp with Node.js/JavaScript? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/whatsapp-gateway-api.html) and start sending images within minutes!

---

**Next Steps**: Once you've mastered basic image sending, explore advanced features like sending [documents](https://www.whatsmate.net/whatsapp-document-individual-api.html) or [group messages](https://www.whatsmate.net/whatsapp-group-message-api.html) through the WhatsMate WA Gateway API documentation.