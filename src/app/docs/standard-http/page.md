---
title: Standard HTTP Monitor  
nextjs:
  metadata:
    title: 'Standard HTTP Monitor Setup - mon1tor'
    description: 'Configure your Standard HTTP Monitor with mon1tor. Understand the key settings like response codes, timeout, and more for effective monitoring.'
---



Standard HTTP Monitoring in mon1tor is a robust tool for ensuring the availability and performance of your web services. This type of monitor checks for successful HTTP responses (status codes in the 2XX range) and alerts you if the responses deviate from this range. This guide details the settings available for configuring a Standard HTTP Monitor.

## Configuration Options

### Basic Settings

1. **Name**: Assign a unique and descriptive name to your monitor for easy identification.
2. **URL**: Enter the URL of the website or web service you want to monitor.
3. **SSL Verification**: Enable or disable SSL certificate verification for your HTTP request. This is crucial for ensuring the security of your HTTPS connections.
4. **Follow Redirect**: Choose whether to follow HTTP redirects. This is useful if your service is expected to return redirects as part of its normal operation.

### Request Settings

1. **Method**: Select the HTTP method to use for the request (e.g., GET, POST, PUT, DELETE).
2. **Request Timeout**: Set the maximum time (in seconds) the monitor will wait for a response before timing out.
3. **Request Headers**: Define any custom headers that your HTTP request should include.
4. **Authentication**: If your service requires authentication, provide the necessary credentials here.

### Monitoring Logic

1. **Number of Checks to Declare Monitor Down**: Specify how many consecutive failed checks (non-2XX responses) are needed before declaring the monitor as 'down'.
2. **Number of Checks to Declare Monitor Up**: Define how many consecutive successful checks are required to switch the monitor's status back to 'up'.

## Setting Up a Standard HTTP Monitor

1. **Navigate to the 'Create Monitor' section** in your mon1tor dashboard.
2. **Fill in the Basic Settings**: Enter the name, URL, and adjust SSL verification and follow redirect options as per your requirements.
3. **Configure the Request Settings**: Choose the method, set the timeout, add any headers, and set up authentication if necessary.
4. **Define the Monitoring Logic**: Set the number of checks for 'down' and 'up' statuses.
5. **Save and activate your monitor**. Your Standard HTTP Monitor is now operational and will alert you based on your configurations.

By fine-tuning these settings, you can tailor your Standard HTTP Monitor to match the specific needs and behavior of your web service, ensuring efficient and reliable monitoring.
