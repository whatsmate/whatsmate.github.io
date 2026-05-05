---
layout: post
title: Convert PDF to Text in VB.NET - Complete Guide
subtitle: Extract text from PDFs using the WhatsMate PDF-to-Text REST API
redirect_from:
  - /2017-06-09-convert-pdf-to-text-vb/
published: true
last_modified_at: 2026-03-16T13:40:00+08:00
---

## Extract Text from PDFs with VB.NET and Visual Studio 2019

Need to extract text from PDF documents programmatically in your VB.NET applications? This guide walks you through converting PDF files to text using VB.NET with Visual Studio 2019 and the WhatsMate PDF-to-Text REST API. Perfect for .NET developers, Windows application builders, and anyone who wants to automate PDF text extraction in their VB.NET-based workflows.

> **Note for Visual Studio 2022 users**: If you're using Visual Studio 2022, please read [this updated tutorial](/2026-03-04-convert-pdf-to-text-vb-vs2022/) instead.


### Prerequisites

Before you begin, ensure you have:

1. **Basic VB.NET knowledge** - Familiarity with VB.NET programming and .NET framework
2. **PDF URL** - A publicly accessible URL to your PDF document
3. **Visual Studio** - .NET development environment (2019 or later)
4. **System.Web.Extensions reference** - Required for JSON serialization


> **Note**: The trial account allows up to 20 PDF-to-Text API calls for learning purposes. Files up to 1 MB can use the synchronous API shown here. [Subscribe to a Premium plan](https://www.whatsmate.net/pdf-api-subscribe.html) for production use and larger files.


### Video Walkthrough

<iframe width="560" height="315" src="https://www.youtube.com/embed/uCU66rDC8eA?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


### Step-by-Step Implementation

Follow these steps to extract text from a PDF using VB.NET:


#### 1. **Copy the VB.NET Code Template**
Start by copying the following source code into your VB.NET Console Application:

{% include gist-styles.html %}

<script src="https://gist.github.com/whatsmate/bc13f03617eddbfe5ce73380ce4c1bc0.js"></script>


#### 2. **Configure the Parameters**
Customize this key parameter in the script:

- **Line 50**: Replace with the URL of your PDF document


#### 3. **Add Required Reference**
Ensure your project references `System.Web.Extensions` for JSON serialization:
1. Right-click on your project in Solution Explorer
2. Select **Add Reference**
3. Find and check **System.Web.Extensions** under Framework
4. Click **OK**


#### 4. **Run the Extraction**
Build and run your VB.NET application in Visual Studio to see the extracted text:
1. Press **F5** to build and run in debug mode
2. Or use **Ctrl+F5** to run without debugging
3. Check the console output for the extracted text


### Common Use Cases

This automation approach is ideal for:
- **Data extraction pipelines** - Pull text from reports, invoices, or forms
- **Content indexing** - Make PDF content searchable in your systems
- **Batch processing** - Extract text from multiple PDFs automatically
- **Integration with workflows** - Add PDF text extraction to .NET applications


### Get Started Today

Ready to automate your PDF text extraction? You'll need an account to access the API. [Sign up for a Premium plan](https://www.whatsmate.net/pdf-api-subscribe.html) and start extracting text within minutes!

---

**Next Steps**: Once you've mastered PDF-to-Text conversion in VB.NET, explore extracting text in other programming languages through the [PDF-to-Text API Getting Started Guide](https://www.whatsmate.net/pdf-to-text-api.html).
