---
layout: post
title: Convert PDF to Text in PHP - Complete Guide
subtitle: Extract text from PDFs using the WhatsMate PDF-to-Text REST API
redirect_from:
  - /2017-06-11-convert-pdf-to-text-php/
published: true
last_modified_at: 2026-03-16T13:40:00+08:00
---

## Extract Text from PDFs with PHP

Need to extract text from PDF documents programmatically in your PHP applications or web scripts? This guide walks you through converting PDF files to text using PHP and the WhatsMate PDF-to-Text REST API. Perfect for PHP developers, web developers, and anyone who wants to automate PDF text extraction in their PHP workflows.


### Prerequisites

Before you begin, ensure you have:

1. **Basic PHP knowledge** - Familiarity with PHP scripts and web servers
2. **PDF URL** - A publicly accessible URL to your PDF document


> **Note**: The trial account allows up to 20 PDF-to-Text API calls for learning purposes. Files up to 1 MB can use the synchronous API shown here. [Subscribe to a Premium plan](https://www.whatsmate.net/pdf-api-subscribe.html) for production use and larger files.


### Step-by-Step Implementation

Follow these steps to extract text from a PDF using PHP:


#### 1. **Copy the Script Template**
Start by copying the following source code into your PHP script file:

{% include gist-styles.html %}

<script src="https://gist.github.com/whatsmate/eb7730ab28c0f29011ebb241d42d0d49.js"></script>


#### 2. **Configure the Parameters**
Customize this key parameter in the script:

- **Line 8**: Replace with the URL of your PDF document


#### 3. **Run the Extraction**
Visit the PHP page in your browser or run it from the command line to see the extracted text:
```bash
php extract-pdf-text-sync.php
```


> ⚠️ **Large PDF files?** If your PDF is larger than 1 MB, you'll need to use the asynchronous API instead. See an [example in PHP](https://github.com/whatsmate/pdf-demos/tree/master/php) for handling larger files.


### Common Use Cases

This automation approach is ideal for:
- **Data extraction pipelines** - Pull text from reports, invoices, or forms
- **Content indexing** - Make PDF content searchable in your systems
- **Batch processing** - Extract text from multiple PDFs automatically
- **Integration with workflows** - Add PDF text extraction to PHP web applications


### Get Started Today

Ready to automate your PDF text extraction? You'll need an account to access the API. [Sign up for a Premium plan](https://www.whatsmate.net/pdf-api-subscribe.html) and start extracting text within minutes!

---

**Next Steps**: Once you've mastered PDF-to-Text conversion in PHP, explore extracting text in other programming languages through the [PDF-to-Text API Getting Started Guide](https://www.whatsmate.net/pdf-to-text-api.html).
