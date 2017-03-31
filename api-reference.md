---
layout: page
title: WhatsMate API Reference
subtitle: WhatsApp Messaging, Telegram Messaging, Translation
---

<br/>

# Table of Contents
* [API Host](#api-host)
* [Common HTTP Header](#common-http-header)
* [Authentication](#authentication)
* [WhatsApp Gateway Endpoints](#whatsapp-gateway-endpoints)
* [Telegram Gateway Endpoints](#telegram-gateway-endpoints)
* [Translation Endpoints](#translation-endpoints)


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

You authenticate yourself against the API server with your `Client ID` and `Client Secret`. You obtain them by subscribing to a premium plan.

They are carried in these HTTP headers: `X-WM-CLIENT-ID` and `X-WM-CLIENT-SECRET`.

Example:
<pre>
X-WM-CLIENT-ID: elsa@example.com
X-WM-CLIENT-SECRET: 53654f8ee3684a37201e3c90a071dbd7
</pre>



<br/>
<hr/>
# WhatsApp Gateway Endpoints

### 1. Check the status of the WhatsApp gateway
* Endpoint: `GET /v1/gateway/status`
* Parameters required: None
* Response: Json containing the following property:
  * `status`: Either "up" or "down"  <br><br>


### 2. Send a WhatsApp message (Deprecated)
* Endpoint: `POST /v1/whatsapp/queue/message`
* Parameters required in JSON payload:
  * `number`: String. The destination phone number including the country code. No "+" sign is needed.
  * `message`: String. The text message that you want to send.
* Response:
  * `{ 'status': 'queued'}`


### 3. Send a WhatsApp message to a single recipient
* Endpoint: `POST /v1/whatsapp/single/message/{instance_number}`
* Parameter required in URL: 
  * `instance_number`: Possible values: 0, 1
* Parameters required in JSON payload:
  * `number`: String. The phone number of the recipient including the country code. No "+" sign is needed.
  * `message`: String. The text message that you want to send.
* Response:
  * `{ 'status': 'queued'}`


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

