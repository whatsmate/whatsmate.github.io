---
layout: post
title: Convert PDF to Text from Shell Script - Complete Guide
subtitle: Extract text from PDFs using the WhatsMate PDF-to-Text REST API
published: true
last_modified_at: 2026-03-05T15:47:00+08:00
---

## Extract Text from PDFs with Shell Scripts

Need to extract text from PDF documents programmatically from your terminal or automation scripts? This guide walks you through converting PDF files to text using a simple shell script and the WhatsMate PDF-to-Text REST API. Perfect for developers, data analysts, and anyone who wants to automate PDF text extraction in their workflows.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **Basic shell scripting knowledge** - Familiarity with terminal commands
2. **PDF URL** - A publicly accessible URL to your PDF document


> ℹ️ **Note**: The trial account allows up to 20 PDF-to-Text API calls for learning purposes. Files up to 1 MB can use the synchronous API shown here. [Subscribe to a Premium plan](https://www.whatsmate.net/pdf-api-subscribe.html) for production use and larger files.


### 📝 Step-by-Step Implementation

Follow these steps to extract text from a PDF using a shell script:


#### 1. **Copy the Script Template**
Start by copying the following source code into your script file:

<script src="https://gist.github.com/whatsmate/6c46d5630b8e154db9600b4457b90837.js"></script>


#### 2. **Configure the Parameters**
Customize this key parameter in the script:

- **Line 9**: Replace with the URL of your PDF document


#### 3. **Make the Script Executable**
Set execute permissions on your script:
```bash
chmod 755 extract-pdf-text-sync.sh
```


#### 4. **Run the Extraction**
Execute the script to see the extracted text:
```bash
./extract-pdf-text-sync.sh
```


> ⚠️ **Large PDF files?** If your PDF is larger than 1 MB, you'll need to use the asynchronous API instead. See an [example in Shell Script](https://github.com/whatsmate/pdf-demos/tree/master/bash) for handling larger files.


### 🔧 Common Use Cases

This automation approach is ideal for:
- **Data extraction pipelines** - Pull text from reports, invoices, or forms
- **Content indexing** - Make PDF content searchable in your systems
- **Batch processing** - Extract text from multiple PDFs automatically
- **Integration with workflows** - Add PDF text extraction to cron jobs or automation scripts


### 🚀 Get Started Today

Ready to automate your PDF text extraction? You'll need an account to access the API. [Sign up for a Premium plan](https://www.whatsmate.net/pdf-api-subscribe.html) and start extracting text within minutes!

---

**Next Steps**: Once you've mastered PDF-to-Text conversion in shell scripts, explore extracting text in other programming languages through the [PDF-to-Text API Getting Started Guide](https://www.whatsmate.net/pdf-to-text-api.html).
