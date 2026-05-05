---
layout: post
title: Convert PDF to Text in Node.js - Complete Guide
subtitle: Extract text from PDFs using the WhatsMate PDF-to-Text REST API
redirect_from:
  - /2017-06-07-convert-pdf-to-text-nodejs/
published: true
last_modified_at: 2026-03-16T13:40:00+08:00
---

## Extract Text from PDFs with Node.js

Need to extract text from PDF documents programmatically in your Node.js applications or scripts? This guide walks you through converting PDF files to text using Node.js and the WhatsMate PDF-to-Text REST API. Perfect for JavaScript developers, backend engineers, and anyone who wants to automate PDF text extraction in their Node.js workflows.


### Prerequisites

Before you begin, ensure you have:

1. **Basic Node.js knowledge** - Familiarity with Node.js scripts and npm
2. **PDF URL** - A publicly accessible URL to your PDF document


> **Note**: The trial account allows up to 20 PDF-to-Text API calls for learning purposes. Files up to 1 MB can use the synchronous API shown here. [Subscribe to a Premium plan](https://www.whatsmate.net/pdf-api-subscribe.html) for production use and larger files.


### Step-by-Step Implementation

Follow these steps to extract text from a PDF using Node.js:


#### 1. **Copy the Script Template**
Start by copying the following source code into your Node.js script file:

{% include gist-styles.html %}

<script src="https://gist.github.com/whatsmate/029ea4925c99b72eb881fb65596d7ece.js"></script>


#### 2. **Configure the Parameters**
Customize this key parameter in the script:

- **Line 10**: Replace with the URL of your PDF document


#### 3. **Make the Script Executable**
Set execute permissions on your script:
```bash
chmod 755 extract-pdf-text-sync.js
```


#### 4. **Run the Extraction**
Execute the script to see the extracted text:
```bash
./extract-pdf-text-sync.js
```


> ⚠️ **Large PDF files?** If your PDF is larger than 1 MB, you'll need to use the asynchronous API instead. See an [example in Node.js](https://github.com/whatsmate/pdf-demos/tree/master/nodejs) for handling larger files.


### Common Use Cases

This automation approach is ideal for:
- **Data extraction pipelines** - Pull text from reports, invoices, or forms
- **Content indexing** - Make PDF content searchable in your systems
- **Batch processing** - Extract text from multiple PDFs automatically
- **Integration with workflows** - Add PDF text extraction to Node.js applications


### Get Started Today

Ready to automate your PDF text extraction? You'll need an account to access the API. [Sign up for a Premium plan](https://www.whatsmate.net/pdf-api-subscribe.html) and start extracting text within minutes!

---

**Next Steps**: Once you've mastered PDF-to-Text conversion in Node.js, explore extracting text in other programming languages through the [PDF-to-Text API Getting Started Guide](https://www.whatsmate.net/pdf-to-text-api.html).
