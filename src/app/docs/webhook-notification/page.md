---
title: Webhook Notification
nextjs:
  metadata:
    title: Configuring Webhook Notifications in mon1tor
    description: Integrate real-time webhook notifications in mon1tor. Learn how to set up and validate your endpoint for secure communication.
---

Webhook notifications in mon1tor offer a dynamic way to integrate alerts into your custom applications or systems. By configuring a webhook, you can receive real-time notifications directly to your specified endpoint. This guide details the setup process for webhook notifications, including endpoint validation and signature verification.

## Configuring Webhook Notifications

1. **Navigate to Settings**: Go to the settings section in your mon1tor dashboard.

2. **Add a URL Endpoint**: Input the URL where you want to receive webhook notifications.

   - **Example**: If your endpoint is `https://www.example.com/webhook/mon1tor`.

3. **Save the Endpoint**: Once you add the URL, mon1tor initiates the validation process.

## Endpoint Validation

- **Token-Based Validation**: To validate the endpoint, mon1tor appends a specific token to your provided URL.

  - **Example**: With a token `123456789`, mon1tor will validate `https://www.example.com/webhook/mon1tor/123456789`.

- **Successful Validation**: The endpoint must reply with a status code in the 2XX range to be considered valid.
  - Once validated, the endpoint is activated, and notifications will begin to be posted to this URL.

## Webhook Security: Secret Key and Signing

- **Automatic Secret Generation**: When a webhook is created, mon1tor automatically generates a secret key.

- **Signature Verification**:
  - Each POST request body sent to your endpoint is signed using SHA256.
  - The hash of the signature is included in the request's POST header with the name `x-mon1tor-sha256-wh`.
  - This mechanism ensures the security and integrity of the data sent to your endpoint.

## Why Use Webhook Notifications?

- **Real-Time Alerts**: Webhooks provide immediate notification delivery, perfect for timely responses.
- **Custom Integration**: Easily integrate alerts into your systems, enabling automated responses or data logging.
- **Security and Integrity**: The signature verification process ensures that the notifications you receive are secure and tamper-proof.

## Summary

Webhook notifications in mon1tor are a powerful tool for integrating real-time alerts into your custom applications or operational workflows. With secure endpoint validation and signature verification, you can trust the reliability and integrity of every alert received.
