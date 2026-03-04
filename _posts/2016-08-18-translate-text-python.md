---
layout: post
title: Translate Text in Python - Complete Guide
subtitle: Automate translations using the WhatsMate Translation REST API
published: true
last_modified_at: 2026-03-04T12:20:00+08:00
---

## Automate Text Translation with Python

Need to translate text programmatically in your Python scripts? This guide walks you through translating text using Python and the WhatsMate Translation REST API. Perfect for Python developers, data scientists, and anyone who wants to integrate automatic translations into their Python projects.


### 📋 Prerequisites

Before you begin, ensure you have:

1. **Python installed** - Python 3 recommended
2. **Requests library** - Install with `pip install requests`
3. **Language codes** - Know the ISO language codes for source and target languages


> ℹ️ **Note**: The trial account allows up to 10 translation API calls for learning purposes. [Subscribe to a Premium plan](https://www.whatsmate.net/translation-subscribe.html) for production use.


### 🎥 Video Walkthrough

<iframe width="560" height="315" src="https://www.youtube.com/embed/qeOQBpYSszA?rel=0&cc_load_policy=1" frameborder="0" allowfullscreen></iframe>


### 📝 Step-by-Step Implementation

Follow these steps to perform your first text translation in Python:


#### 1. **Copy the Script Template**
Start by copying the following source code into your Python script:

<script src="https://gist.github.com/whatsmate/c0faa349997272fc74b18f2cbb8ece66.js"></script>


#### 2. **Configure the Parameters**
Customize these key parameters in the script:

- **Line 10**: Replace with the source language code (e.g., `en` for English)
- **Line 11**: Replace with the target language code (e.g., `pt` for Portuguese)
- **Line 12**: Provide the text you want to translate


> 🔍 **Looking for language codes?** See the [complete listing of supported language codes](http://api.whatsmate.net/v1/translation/supported-codes).


#### 3. **Install Dependencies**
Install the required Requests library:
```bash
pip install requests
```


#### 4. **Make the Script Executable**
Set execute permissions on your script:
```bash
chmod 755 translate-text.py
```


#### 5. **Run the Translation**
Execute the script to see the translated result:
```bash
./translate-text.py
```


### 🔧 Common Use Cases

This automation approach is ideal for:
- **Data analysis** - Translate text data in pandas DataFrames
- **Machine learning pipelines** - Preprocess multilingual datasets
- **Web scraping** - Translate scraped content automatically
- **Chatbots and NLP** - Build multilingual conversational agents
- **Automation scripts** - Translate notifications and reports


### 🚀 Get Started Today

Ready to automate your text translations? You'll need an account to access the API. [Sign up for a Premium plan](https://www.whatsmate.net/translation-subscribe.html) and start translating within minutes!

---

**Next Steps**: Once you've mastered basic text translation, explore translating text in other programming languages through the [Translation API Getting Started Guide](https://www.whatsmate.net/translation-api.html).

