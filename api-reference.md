---
layout: page
title: WhatsMate API Reference
subtitle: WhatsApp Messaging, Telegram Messaging, Translation, PDF-to-Text
---

<br/>

# Table of Contents
* [API Host](#api-host)
* [Common HTTP Header](#common-http-header)
* [Authentication](#authentication)
* [WhatsApp Gateway Endpoints](#whatsapp-gateway-endpoints)
* [Telegram Gateway Endpoints](#telegram-gateway-endpoints)
* [Translation Endpoints](#translation-endpoints)
* [PDF-to-Text Endpoints](#pdf-to-text-endpoints)


<br/>
<hr/>
## API Host

All REST API endpoints are hosted on `http://api.whatsmate.net/`.

If you prefer `https`, you can use `https://api.whatsmate.net/`.


<br/>
<hr/>
## Common HTTP header

You should include the following HTTP header in your call to any one of the endpoints:

- `Content-Type: application/json`


<br/>
<hr/>
## Authentication

You authenticate yourself against the API server with your `Client ID` and `Client Secret`. You obtain them by subscribing to a Premium plan of the service you intend to use.

They are carried in these HTTP headers: `X-WM-CLIENT-ID` and `X-WM-CLIENT-SECRET`.

Example:
<pre>
X-WM-CLIENT-ID: elsa@example.com
X-WM-CLIENT-SECRET: 53654f8ee3684a37201e3c90a071dbd7
</pre>



<br/>
<hr/>
# WhatsApp Gateway Endpoints

&nbsp;

## ![Download source code](/img/download-run.png) Demo App

Check out the [wa-demos](https://github.com/whatsmate/wa-demos) repository to see how the APIs are called.

&nbsp;


### 1. Check the status of the WhatsApp gateway
* Endpoint: `GET /v1/gateway/status`
* Parameters required: None
* Response: Json containing the following property:
  * `status`: Either "up" or "down"  <br><br>


### 2. Send a WhatsApp message to a single recipient
* Endpoint: `POST /v3/whatsapp/single/text/message/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: An integer indicating your gateway's instance ID
* Parameters required in JSON payload:
  * `number`: String. The phone number of the recipient including the country code. No "+" sign is needed.
  * `message`: String. The text message that you want to send.
* Response:
  * `{ 'status': 'queued', 'id': '<Job ID>'}`


### 3. Send a message to a WhatsApp Group that the gateway participates in
* Endpoint: `POST /v3/whatsapp/group/text/message/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: An integer indicating your gateway's instance ID
* Parameters required in JSON payload:
  * `group_name`: String. The name of the WhatsApp group.
  * `group_admin`: String. The phone number (including the country code) of the group creator. No "+" sign is needed.
  * `message`: String. The text message that you want to send.
* Response:
  * `{ 'status': 'queued', 'id': '<Job ID>'}`


<br/>
<hr/>
# Telegram Gateway Endpoints

&nbsp;

## ![Download source code](/img/download-run.png)  Demo App

Check out the [telegram-demos](https://github.com/whatsmate/telegram-demos) repository to see how the APIs are called.

&nbsp;


### 1. Check the status of the Telegram gateway
* Endpoint: `GET /v1/telegram/status/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: Possible value: 0
* Response: Json containing the following properties:
  * `status`: Either "up" or "down"
  * `instance`: The instance number of the gateway
* Example request: `GET /v1/telegram/status/0`  <br><br>


### 2. Send a Telegram message to a single recipient
* Endpoint: `POST /v1/telegram/single/message/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: Possible value: 0
* Parameters required in JSON payload:
  * `number`: String. The phone number of the recipient including the country code. No "+" sign is needed.
  * `message`: String. The text message that you want to send.
* Response: Json containing these properties:
  * `success`: Possible values: `true` / `false`
  * `status`: String. Text explaining what happened.


### 3. (Premium Only) Send a Telegram message to multiple recipients
* Endpoint: `POST /v1/telegram/batch/message/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: Possible value: 0
* Parameters required in JSON payload:
  * `numbers`: Array of strings. The phone numbers of the recipients including the country code. No "+" sign is needed.
  * `message`: String. The text message that you want to send.
* Response: Json containing these properties:
  * `success`: Possible values: `true` / `false`
  * `status`: String. Text explaining what happened.


### 4. Send a location to a single recipient
* Endpoint: `POST /v1/telegram/single/location/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: Possible value: 0
* Parameters required in JSON payload:
  * `number`: String. The phone number of the recipient including the country code. No "+" sign is needed.
  * `latitude`: Number. The latitude of the location that you want to send.
  * `longitude`: Number. The longitude of the location that you want to send.
* Response: Json containing these properties:
  * `success`: Possible values: `true` / `false`
  * `status`: String. Text explaining what happened.


### 5. (Premium Only) Send a location to multiple recipients
* Endpoint: `POST /v1/telegram/batch/location/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: Possible value: 0
* Parameters required in JSON payload:
  * `numbers`: Array of strings. The phone numbers of the recipients including the country code. No "+" sign is needed.
  * `latitude`: Number. The latitude of the location that you want to send.
  * `longitude`: Number. The longitude of the location that you want to send.
* Response: Json containing these properties:
  * `success`: Possible values: `true` / `false`
  * `status`: String. Text explaining what happened.


### 6. (Premium Only) Send a photo/image to a single recipient
* Endpoint: `POST /v1/telegram/single/photo/binary/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: Possible value: 0
* Parameters required in JSON payload:
  * `number`: String. The phone number of the recipient including the country code. No "+" sign is needed.
  * `image`: String. Base64-encoded representation of the image that you want to send.
  * `caption`: String. Optional. A short description of your image.
* Response: Json containing these properties:
  * `success`: Possible values: `true` / `false`
  * `status`: String. Text explaining what happened.


### 7. (Premium Only) Send a photo/image to multiple recipients
* Endpoint: `POST /v1/telegram/batch/photo/binary/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: Possible value: 0
* Parameters required in JSON payload:
  * `numbers`: Array of strings. The phone numbers of the recipients including the country code. No "+" sign is needed.
  * `image`: String. Base64-encoded representation of the image that you want to send.
  * `caption`: String. Optional. A short description of your image.
* Response: Json containing these properties:
  * `success`: Possible values: `true` / `false`
  * `status`: String. Text explaining what happened.


### 8. (Premium Only) Send an audio file to a single recipient
* Endpoint: `POST /v1/telegram/single/audio/binary/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: Possible value: 0
* Parameters required in JSON payload:
  * `number`: String. The phone number of the recipient including the country code. No "+" sign is needed.
  * `audio`: String. Base64-encoded representation of the audio content that you want to send.
  * `filename`: String. The filename of your audio file.
* Response: Json containing these properties:
  * `success`: Possible values: `true` / `false`
  * `status`: String. Text explaining what happened.


### 9. (Premium Only) Send an audio file to multiple recipients
* Endpoint: `POST /v1/telegram/batch/audio/binary/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: Possible value: 0
* Parameters required in JSON payload:
  * `numbers`: Array of strings. The phone numbers of the recipients including the country code. No "+" sign is needed.
  * `audio`: String. Base64-encoded representation of the audio content that you want to send.
  * `filename`: String. The filename of your audio file.
* Response: Json containing these properties:
  * `success`: Possible values: `true` / `false`
  * `status`: String. Text explaining what happened.


### 10. (Premium Only) Send a document (e.g. PDF) to a single recipient
* Endpoint: `POST /v1/telegram/single/document/binary/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: Possible value: 0
* Parameters required in JSON payload:
  * `number`: String. The phone number of the recipient including the country code. No "+" sign is needed.
  * `document`: String. Base64-encoded representation of the document content that you want to send.
  * `filename`: String. The filename of your document file.
* Response: Json containing these properties:
  * `success`: Possible values: `true` / `false`
  * `status`: String. Text explaining what happened.


### 11. (Premium Only) Send a document (e.g. PDF) to multiple recipients
* Endpoint: `POST /v1/telegram/batch/document/binary/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: Possible value: 0
* Parameters required in JSON payload:
  * `numbers`: Array of strings. The phone numbers of the recipients including the country code. No "+" sign is needed.
  * `document`: String. Base64-encoded representation of the document content that you want to send.
  * `filename`: String. The filename of your document file.
* Response: Json containing these properties:
  * `success`: Possible values: `true` / `false`
  * `status`: String. Text explaining what happened.


### 12. (Premium Only) Send a Telegram message to a group
* Endpoint: `POST /v1/telegram/group/message/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: Possible value: 0
* Parameters required in JSON payload:
  * `group`: String. The name of the group that the gateway is part of.
  * `message`: String. The text message that you want to send.
* Response: Json containing these properties:
  * `success`: Possible values: `true` / `false`
  * `status`: String. Text explaining what happened.


<br/>
<hr/>
# Translation Endpoints

### 1. Translate text
* Endpoint: `POST /v1/translation/translate`
* Parameters required in JSON payload:
  * `fromLang`: String. The code representing the language of the supplied text.
  * `toLang`: String. The code representing the language you want the text to be translated to.
  * `text`: String. The piece of text you want to be translated.
* List of lanugage codes: See the next endpoint.
* Response: String. The translated text.  <br><br>


### 2. List all the possible language codes
* Endpoint: `GET /v1/translation/supported-codes`
* Parameters required: None
* Response: JSON showing all the possible language codes.


<br/>
<hr/>
# PDF-to-Text Endpoints

### 1. Extract text from a PDF file synchronously
* Endpoint: `GET /v1/pdf/extract`
* Query String parameter required:
  * `url`: String. The URL of the PDF file that you want to extract the text of.
* Response: String. The extracted text  <br><br>


### 2. Submit a job to extract text asynchronously
* Endpoint: `GET /v1/pdf/job/submit`
* Query String parameter required:
  * `url`: String. The URL of the PDF file that you want to extract the text of.
* Response: Json containing these properties:
  * `id`: String. ID of the job that you have submitted
  * `status`: String. Text describing the current state of the job
<br><br>


### 3. Check the status of a specific job
* Endpoint: `GET /v1/pdf/job/check/<jobId>`
* Parameter as part of the URI path:
  * `jobId`: String. ID of the job that you want to check the status of.
* Response: Json containing these properties:
  * `id`: String. ID of the job being queried.
  * `status`: String. Text describing the current state of the job
<br><br>


### 4. Retrieve the PDF text from a completed job
* Endpoint: `GET /v1/pdf/job/retrieve_text/<jobId>`
* Parameter as part of the URI path:
  * `jobId`: String. ID of the job that you want to check the status of.
* Response: String. The extracted text  <br><br>

