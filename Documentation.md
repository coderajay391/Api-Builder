# API Builder — Documentation

## Overview

**API Builder** helps you quickly design, test, and document API endpoints. It focuses on making the API development loop (define → test → document) faster and more consistent.

## Core Concepts

### 1) Endpoint

An **endpoint** describes how to call an API:

- **Method**: `GET`, `POST`, `PUT`, `PATCH`, `DELETE`
- **Path**: URL path (e.g., `/users`, `/products/:id`)
- **Headers**: optional headers like `Authorization`, `Content-Type`
- **Body / Payload**: JSON or other request payloads (for methods that support bodies)
- **Query Params**: key/value pairs appended to the URL

### 2) Request Test

Run a request and inspect:

- HTTP status code (e.g., 200, 201, 400)
- Response body (JSON/text)
- Response headers (optional)

### 3) Export / Documentation

Save endpoint details so you (or your team) can reuse them later.

## Getting Started

> If the project is an npm-based app, install and run it as follows:

1. Install dependencies:
   - `npm install`
2. Start the project:
   - `npm start`
   - or `npm run dev`

## How to Use

### Step 1: Create an endpoint

- Choose the HTTP method
- Enter the endpoint path
- Add query parameters if needed

### Step 2: Configure headers

- Add `Content-Type: application/json` when sending JSON
- Add `Authorization` or other headers if required

### Step 3: Send a request

- Provide the payload (if applicable)
- Click **Send / Test**
- Review the response output

### Step 4: Save your endpoint

- Store the configuration (method, path, headers, body)
- Optionally add notes for expected behavior

## Request / Response Guidelines

### Request payload

- Use valid JSON
- Match the API’s expected schema
- Keep field names consistent with backend expectations

### Response validation (recommended)

When possible, compare response shapes against:

- expected status codes
- required keys (e.g., `data`, `message`, `error`)

## Typical Use Cases

- Building a new REST API
- Testing endpoints during development
- Creating simple API docs for a demo or internal use

## Troubleshooting

- **401/403**: Check `Authorization` header and token expiration
- **400**: Validate JSON syntax and required fields
- **404**: Confirm the endpoint path and method match

## Notes

This documentation is intentionally brief. Extend it as the project gains more features (auth flows, collections, environments, etc.).
