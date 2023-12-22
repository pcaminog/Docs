---
title: Integrations Notification
---

mon1tor provides seamless integration with popular communication platforms: Slack, Google Chat, and Microsoft Teams. These integrations enable you to receive alerts directly in your team's communication channels, enhancing the speed and efficiency of your response. This guide outlines the steps to set up notifications for each platform.

## Slack Integration

- **mon1tor App for Slack**: We have developed a mon1tor app that can be integrated into any Slack channel.
- **Setup Process**:
  1. Go to the settings in your mon1tor dashboard.
  2. At the bottom of the page, follow the instructions to add the mon1tor app to your desired Slack channel through OAuth2.

## Google Chat Integration

- **Setting Up Webhooks in Google Chat**:
  1. In a browser, open Google Chat (Webhooks are not configurable from the mobile app).
  2. Navigate to the space where you want to add the webhook.
  3. Click on the "Apps & integrations" option near the space title.
  4. Choose "Add webhooks".
  5. Enter "mon1tor Webhook" as the name and use `https://static.mon1tor.com/logo+name.svg` for the Avatar URL.
  6. Save and copy the webhook URL provided. This URL will be used in mon1tor to send notifications to your Google Chat space.

## Microsoft Teams Integration

- **Adding Incoming Webhook to Teams**:
  1. Open the channel in Teams where you want to add the webhook.
  2. Select "Connectors" from the dropdown menu in the upper-right corner.
  3. Search for and select "Incoming Webhook", then choose "Configure".
  4. Provide a name for your webhook and upload an image if necessary.
  5. Create the webhook and save the unique URL provided.
  6. This URL will be used in mon1tor to send notifications to your Microsoft Teams channel.

## Summary

Integrating mon1tor notifications with Slack, Google Chat, and Microsoft Teams enables efficient and immediate communication of alerts within your team's existing collaboration platforms. By following these setup processes, you can ensure that your team is always promptly informed about the status of your monitors.
