---
title: Code HTTP Monitor  
nextjs:
  metadata:
    title: Code HTTP Monitor Configuration - mon1tor
    description: Set up a Code HTTP Monitor with mon1tor to track specific HTTP response codes. Customize your monitoring for redirects, errors, and more.
---


The Code HTTP Monitor in mon1tor offers a flexible approach to HTTP monitoring by allowing you to specify the expected HTTP response codes. This feature is particularly useful for monitoring redirects, error pages, or any other specific HTTP responses. The guide below outlines the settings and steps to configure a Code HTTP Monitor.

## Configuration Options

### Basic Settings

1. **Name**: Give your monitor a unique and descriptive name.
2. **URL**: Enter the URL of the site or service to be monitored.
3. **Status Code**: Enter the HTTP status code expected to receive.

### Advanced Settings

1. **Expected HTTP Code(s)**: Define the specific HTTP status code(s) you expect to receive. This could be any valid HTTP response code like 301, 404, 200, etc.

2. **SSL Verification**: Toggle SSL certificate verification for HTTPS connections.

3. **Follow Redirects**: Decide whether the monitor should follow redirects. Useful if you are specifically monitoring for redirect responses.

### Request Configuration

1. **Method**: Choose the HTTP method (GET, POST, etc.) for your request.

2. **Request Timeout**: Set a time limit for how long the monitor waits for a response.

3. **Request Headers**: Include any necessary custom headers for your HTTP request.

4. **Authentication**: Provide credentials if the monitored service requires authentication.

### Monitoring Logic

1. **Number of Checks to Declare Monitor Down**: Set the number of consecutive checks that must fail (not receive the expected HTTP code) to consider the monitor down.

2. **Number of Checks to Declare Monitor Up**: Indicate how many consecutive successful checks (receiving the expected HTTP code) are needed for the monitor to be considered up.

## Setting Up a Code HTTP Monitor

1. **Go to 'Create Monitor'** in your mon1tor dashboard.

2. **Enter Basic Settings**: Input the name and URL.

3. **Specify the Expected HTTP Code(s)** in the Advanced Settings.

4. **Configure your Request**: Choose the method, set the timeout, add headers, and set up authentication as needed.

5. **Determine the Monitoring Logic**: Decide on the number of checks for down and up statuses.

6. **Activate the monitor**. Your Code HTTP Monitor is now set to alert you based on the specified HTTP response codes.

This specialized monitoring tool ensures that you have precise control over the HTTP responses you expect, enabling tailored monitoring for specific scenarios and requirements.
