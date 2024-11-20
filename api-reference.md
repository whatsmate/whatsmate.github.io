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

You should always include the following HTTP header in your calls to our endpoints:

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


### 1. Send a WhatsApp text message to a single recipient
* Endpoint: `POST /v3/whatsapp/single/text/message/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: An integer indicating your gateway's instance ID
* Parameters required in `JSON` payload:
  * `number`: String. The phone number of the recipient including the country code. No "+" sign is needed.
  * `message`: String. The text message that you want to send.
* Response:
  * `{ 'status': 'queued', 'id': '<Job ID>'}`
* Code Examples:
  * [Follow this guide](https://www.whatsmate.net/whatsapp-gateway-api.html).

&nbsp;


### 2. Send a text message to a WhatsApp Group that the gateway participates in
* Endpoint: `POST /v3/whatsapp/group/text/message/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: An integer indicating your gateway's instance ID
* Parameters required in `JSON` payload:
  * `group_name`: String. The name of the WhatsApp group.
  * `group_admin`: String. The phone number (including the country code) of the group creator. No "+" sign is needed.
  * `message`: String. The text message that you want to send.
* Response:
  * `{ 'status': 'queued', 'id': '<Job ID>'}`
* Code Examples:
  * [Follow this guide](https://www.whatsmate.net/whatsapp-group-message-api.html).

&nbsp;


### 3. Send a photo/image to a single recipient
* Endpoint: `POST /v3/whatsapp/single/image/message/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: An integer indicating your gateway's instance ID
* Parameters required in `JSON` payload:
  * `number`: String. The phone number of the recipient including the country code. No "+" sign is needed.
  * `image`: String. Base64-encoded representation of the image that you want to send.
  * `caption`: String - optional field. A short description that goes with the image.
* Response: Json containing these properties:
  * `{ 'status': 'queued', 'id': '<Job ID>'}`
* Code Examples:
  * [Follow this guide](https://www.whatsmate.net/whatsapp-image-individual-api.html).

&nbsp;


### 4. Send a photo/image to a WhatsApp group that the gateway participates in
* Endpoint: `POST /v3/whatsapp/group/image/message/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: An integer indicating your gateway's instance ID
* Parameters required in `JSON` payload:
  * `group_name`: String. The name of the WhatsApp group.
  * `image`: String. Base64-encoded representation of the image that you want to send.
  * `caption`: String - optional field. A short description that goes with the image.
* Response: Json containing these properties:
  * `{ 'status': 'queued', 'id': '<Job ID>'}`
* Code Examples:
  * [Follow this guide](https://www.whatsmate.net/whatsapp-group-image-api.html).

&nbsp;


### 5. Send a document (e.g. PDF, MP3, etc.) to a single recipient
* Endpoint: `POST /v3/whatsapp/single/document/message/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: An integer indicating your gateway's instance ID
* Parameters required in `JSON` payload:
  * `number`: String. The phone number of the recipient including the country code. No "+" sign is needed.
  * `document`: String. Base64-encoded representation of the document that you want to send.
  * `filename`: String. Name of the file that will be presented to the receiver.
* Response: Json containing these properties:
  * `{ 'status': 'queued', 'id': '<Job ID>'}`
* Code Examples:
  * [Follow this guide](https://www.whatsmate.net/whatsapp-document-individual-api.html).

&nbsp;


### 6. Send a document (e.g. PDF, MP3, etc.) to a WhatsApp group that the gateway participates in
* Endpoint: `POST /v3/whatsapp/group/document/message/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: An integer indicating your gateway's instance ID
* Parameters required in `JSON` payload:
  * `group_name`: String. The name of the WhatsApp group.
  * `document`: String. Base64-encoded representation of the document that you want to send.
  * `filename`: String. Name of the file that will be presented to the receiver.
* Response: Json containing these properties:
  * `{ 'status': 'queued', 'id': '<Job ID>'}`
* Code Examples:
  * [Follow this guide](https://www.whatsmate.net/whatsapp-group-document-api.html).

&nbsp;


<br/>
<br/>
<hr/>
# Telegram Gateway Endpoints

&nbsp;

## ![Download source code](/img/download-run.png)  Demo App

Check out the [telegram-demos](https://github.com/whatsmate/telegram-demos) repository to see how the APIs are called.

&nbsp;


### 1. Send a Telegram text message to a single recipient
* Endpoint: `POST /v3/telegram/single/text/message/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: An integer indicating your gateway's instance ID
* Parameters required in `JSON` payload:
  * `number`: String. The phone number of the recipient including the country code. No "+" sign is needed.
  * `message`: String. The text message that you want to send.
* Response:
  * `{ 'status': 'queued', 'id': '<Job ID>'}`
* Code Examples:
  * [Follow this guide](https://www.whatsmate.net/telegram-gateway-api.html).

&nbsp;


### 2. Send a text message to a Telegram Group that the gateway participates in
* Endpoint: `POST /v3/telegram/group/text/message/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: An integer indicating your gateway's instance ID
* Parameters required in `JSON` payload:
  * `group_name`: String. The name of the Telegram group.
  * `group_admin`: String. The phone number (including the country code) of the group creator. No "+" sign is needed.
  * `message`: String. The text message that you want to send.
* Response:
  * `{ 'status': 'queued', 'id': '<Job ID>'}`
* Code Examples:
  * [Follow this guide](https://www.whatsmate.net/telegram-group-message-api.html).

&nbsp;


### 3. Send a photo/image to a single recipient
* Endpoint: `POST /v3/telegram/single/image/message/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: An integer indicating your gateway's instance ID
* Parameters required in `JSON` payload:
  * `number`: String. The phone number of the recipient including the country code. No "+" sign is needed.
  * `image`: String. Base64-encoded representation of the image that you want to send.
  * `caption`: String - optional field. A short description that goes with the image.
* Response: Json containing these properties:
  * `{ 'status': 'queued', 'id': '<Job ID>'}`
* Code Examples:
  * [Follow this guide](https://www.whatsmate.net/telegram-image-individual-api.html).

&nbsp;


### 4. Send a photo/image to a Telegram group that the gateway participates in
* Endpoint: `POST /v3/telegram/group/image/message/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: An integer indicating your gateway's instance ID
* Parameters required in `JSON` payload:
  * `group_name`: String. The name of the Telegram group.
  * `group_admin`: String. The phone number (including the country code) of the group creator. No "+" sign is needed.
  * `image`: String. Base64-encoded representation of the image that you want to send.
  * `caption`: String - optional field. A short description that goes with the image.
* Response: Json containing these properties:
  * `{ 'status': 'queued', 'id': '<Job ID>'}`
* Code Examples:
  * [Follow this guide](https://www.whatsmate.net/telegram-group-image-api.html).

&nbsp;


### 5. Send a document (e.g. PDF, etc.) to a single recipient
* Endpoint: `POST /v3/telegram/single/document/message/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: An integer indicating your gateway's instance ID
* Parameters required in `JSON` payload:
  * `number`: String. The phone number of the recipient including the country code. No "+" sign is needed.
  * `document`: String. Base64-encoded representation of the document that you want to send.
  * `filename`: String. Name of the file that will be presented to the receiver.
  * `caption`: String - optional field. A short description that goes with the document.
* Response: Json containing these properties:
  * `{ 'status': 'queued', 'id': '<Job ID>'}`
* Code Examples:
  * [Follow this guide](https://www.whatsmate.net/telegram-document-individual-api.html).

&nbsp;


### 6. Send a document (e.g. PDF, etc.) to a Telegram group that the gateway participates in
* Endpoint: `POST /v3/telegram/group/document/message/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: An integer indicating your gateway's instance ID
* Parameters required in `JSON` payload:
  * `group_name`: String. The name of the Telegram group.
  * `group_admin`: String. The phone number (including the country code) of the group creator. No "+" sign is needed.
  * `document`: String. Base64-encoded representation of the document that you want to send.
  * `filename`: String. Name of the file that will be presented to the receiver.
  * `caption`: String - optional field. A short description that goes with the document.
* Response: Json containing these properties:
  * `{ 'status': 'queued', 'id': '<Job ID>'}`
* Code Examples:
  * [Follow this guide](https://www.whatsmate.net/telegram-group-document-api.html).

&nbsp;


### 7. Send an audio file (e.g. MP3) to a single recipient
* Endpoint: `POST /v3/telegram/single/audio/message/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: An integer indicating your gateway's instance ID
* Parameters required in `JSON` payload:
  * `number`: String. The phone number of the recipient including the country code. No "+" sign is needed.
  * `audio`: String. Base64-encoded representation of the audio file that you want to send.
  * `filename`: String. Name of the file that will be presented to the receiver.
  * `caption`: String - optional field. A short description that goes with the audio file.
* Response: Json containing these properties:
  * `{ 'status': 'queued', 'id': '<Job ID>'}`
* Code Examples:
  * [Follow this guide](https://www.whatsmate.net/telegram-audio-individual-api.html).

&nbsp;


### 8. Send an audio file (e.g. MP3) to a Telegram group that the gateway participates in
* Endpoint: `POST /v3/telegram/group/audio/message/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: An integer indicating your gateway's instance ID
* Parameters required in `JSON` payload:
  * `group_name`: String. The name of the Telegram group.
  * `group_admin`: String. The phone number (including the country code) of the group creator. No "+" sign is needed.
  * `audio`: String. Base64-encoded representation of the audio file that you want to send.
  * `filename`: String. Name of the file that will be presented to the receiver.
  * `caption`: String - optional field. A short description that goes with the audio file.
* Response: Json containing these properties:
  * `{ 'status': 'queued', 'id': '<Job ID>'}`
* Code Examples:
  * [Follow this guide](https://www.whatsmate.net/telegram-audio-document-api.html).

&nbsp;


### 9. Send a voice note file (e.g. opus) to a single recipient
* Endpoint: `POST /v3/telegram/single/voice_note/message/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: An integer indicating your gateway's instance ID
* Parameters required in `JSON` payload:
  * `number`: String. The phone number of the recipient including the country code. No "+" sign is needed.
  * `voice_note`: String. Base64-encoded representation of the voice note file that you want to send.
  * `filename`: String. Name of the file that will be presented to the receiver.
  * `caption`: String - optional field. A short description that goes with the voice note file.
* Response: Json containing these properties:
  * `{ 'status': 'queued', 'id': '<Job ID>'}`
* Code Examples:
  * [Follow this guide](https://www.whatsmate.net/telegram-voice-note-individual-api.html).

&nbsp;


### 10. Send a voice note file (e.g. opus) to a Telegram group that the gateway participates in
* Endpoint: `POST /v3/telegram/group/voice_note/message/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: An integer indicating your gateway's instance ID
* Parameters required in `JSON` payload:
  * `group_name`: String. The name of the Telegram group.
  * `group_admin`: String. The phone number (including the country code) of the group creator. No "+" sign is needed.
  * `voice_note`: String. Base64-encoded representation of the voice note file that you want to send.
  * `filename`: String. Name of the file that will be presented to the receiver.
  * `caption`: String - optional field. A short description that goes with the voice note file.
* Response: Json containing these properties:
  * `{ 'status': 'queued', 'id': '<Job ID>'}`
* Code Examples:
  * [Follow this guide](https://www.whatsmate.net/telegram-group-voice-note-api.html).

&nbsp;



<br/>
<hr/>
# Translation Endpoints

### 1. Translate text
* Endpoint: `POST /v1/translation/translate`
* Parameters required in `JSON` payload:
  * `fromLang`: String. The code representing the language of the supplied text.
  * `toLang`: String. The code representing the language you want the text to be translated to.
  * `text`: String. The piece of text you want to be translated.
* List of lanugage codes: See the next endpoint.
* Response: String. The translated text.  <br><br>


### 2. List all the possible language codes
* Endpoint: `GET /v1/translation/supported-codes`
* Parameters required: None
* Response: `JSON` showing all the possible language codes.


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

