---
layout: post
title: Send PDF Files over WhatsApp in Java - Complete Guide
subtitle: Automate WhatsApp document sharing using the WhatsMate WA Gateway REST API
published: true
last_modified_at: 2026-02-12T12:45:00+08:00
---

## Automate WhatsApp Document Sharing with Java

Looking to automate PDF delivery, document notifications, or file sharing from your Java applications? This guide walks you through sending PDF files to WhatsApp users using Java and the WhatsMate WA Gateway REST API. Perfect for Java developers, system administrators, and automation enthusiasts who want to integrate document delivery into their Java-based WhatsApp messaging workflows.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **A WhatsMate WA Gateway account** - Required for API access
2. **Recipient registration** - Each recipient must register with the Gateway first
3. **Java development environment** - JDK installed and configured
4. **PDF file ready** - Have the document you want to send available locally
5. **Required libraries** - Gson and Commons Codec (details in code comments)

> ⚠️ **Important**: Recipients must register with the WhatsMate WA Gateway before they can receive messages. Unregistered users will not receive any messages from the Gateway. Registration instructions are available on the [official WhatsMate site](https://www.whatsmate.net/whatsapp-gateway-api.html).


### 📝 Step-by-Step Implementation

Follow these steps to send your first PDF document to a WhatsApp user from a Java application:


#### 1. **Copy the Java Code Template**
Start by copying the following source code into your Java file:

<script src="https://gist.github.com/whatsmate/8e034dc5e92ca402436818a5c7701894.js"></script>


#### 2. **Configure a few Parameters**
Customize these key parameters in the Java code:

- **Line 50**: Replace `YOUR_INSTANCE_ID_HERE` with your WhatsApp gateway instance ID
- **Lines 51-52**: Update `YOUR_CLIENT_ID_HERE` and `YOUR_CLIENT_SECRET_HERE` with your Client ID and Secret
- **Line 61**: Replace `1234556899` with the target phone number (including the country code)
- **Line 63**: Replace `../assets/subwaymap.pdf` with the path to your PDF file
- **Line 65**: Replace `anyname.pdf` with the desired filename for the document
- **Line 66**: Replace `You will find the map handy.` with an optional caption for your PDF


#### 3. **Compile the Java Program**
You can compile and run the program using either Maven or manual compilation:

**Option A: Using Maven**
Add the following dependencies to your `pom.xml`:
```xml
<dependency>
    <groupId>com.google.code.gson</groupId>
    <artifactId>gson</artifactId>
    <version>2.8.0</version>
</dependency>
<dependency>
    <groupId>commons-codec</groupId>
    <artifactId>commons-codec</artifactId>
    <version>1.10</version>
</dependency>
```
Then compile with Maven:
```bash
mvn compile
```

**Option B: Manual Compilation**
If not using Maven, compile with:
```bash
javac -cp "jars/gson-2.8.0.jar:jars/commons-codec-1.10.jar" WaPdfSender.java
```


#### 4. **Send Your PDF Document**
Run the compiled Java program to deliver your PDF to WhatsApp:

**If using Maven:**
```bash
mvn exec:java -Dexec.mainClass="WaPdfSender"
```

**If using manual compilation:**
```bash
java -cp ".:jars/gson-2.8.0.jar:jars/commons-codec-1.10.jar" WaPdfSender
```


### 🔧 Common Use Cases

This automation approach is ideal for:
- **Automated report delivery** - Send daily/weekly PDF reports to WhatsApp from Java applications
- **Document sharing automation** - Deliver invoices, receipts, or contracts via WhatsApp using Java
- **System documentation** - Share configuration files or logs as PDF documents from Java systems
- **Educational content** - Distribute learning materials or tutorials through WhatsApp from Java
- **Integration with Java document generation** - Combine with Java libraries that create PDFs for WhatsApp delivery


### 🚀 Get Started Today

Ready to automate your document sharing over WhatsApp with Java? You'll need a trial account to access the API. [Sign up for a 2-week trial](https://www.whatsmate.net/whatsapp-gateway-api.html) and start sending PDF files within minutes!

---

**Next Steps**: Once you've mastered basic PDF sending, explore advanced features like sending [images](https://www.whatsmate.net/whatsapp-image-individual-api.html) or [group messages](https://www.whatsmate.net/whatsapp-group-message-api.html) through the WhatsMate WA Gateway API documentation.