# Manic Host REST API

> **API Endpoint:** https://api.manic.host/

## Getting your API key
Login to your account at [Manic Host](https://my.manic.host) and visit your **Settings** page. On this page, you'll see the API Key field.

<img src="http://manic.host/images/api-step-1.png" />

Click the **Reveal** button to see your API key.

<img src="http://manic.host/images/api-step-2.png" />

Keep your API key safe.

## Making requests
After obtaining your API key, you may immediately make API requests to the primary API endpoint.

When sending requests, the **X_API_KEY** header should be set with your API key as the value. This is the only authentication required.

By default, responses are returned in XML format. If you would like to have responses returned as JSON, you should send the _Accept: application/json_ header.

In addition to the listed response parameters, the _status_ parameter will be returned as a boolean representation of the successfulness of the request.

## Methods

[Domains](https://github.com/iann0036/ManicHostREST/blob/master/Domains.md)

[Hosting](https://github.com/iann0036/ManicHostREST/blob/master/Hosting.md)

### GET /
Returns metadata about the API service.

#### Request
There are no request parameters for this method.

#### Response
- _api_version_ - The active version of the API
- _documentation_ - Link to the latest documentation of the API
