---
title: What is an Alert?
nextjs:
  metadata:
    title: 'Understanding Alerts in mon1tor - Notification Insights'
    description: 'Learn when and how alerts are generated in mon1tor, how they are associated with your monitors, and the notification process involved.'
---

In mon1tor, an alert is a crucial notification mechanism that informs you of any issues detected with your monitored services. Alerts are generated based on specific conditions set in your monitor configurations. This page explains when and how alerts are triggered, their components, and the notification process.

## Alert Generation

An alert in mon1tor is triggered under the following condition:

- **Number of Consecutive Failures**: When the number of consecutive checks that fail reaches the threshold set in the 'Number of Checks to Declare Monitor Down', an alert is generated. This applies to both HTTP and DNS monitors.

### Components of an Alert

1. **Alert ID**: Each alert is assigned a unique identifier for tracking and reference.

2. **Error Detail**:
   - For HTTP monitors, this includes the HTTP response code and status.
   - For DNS monitors, it details the DNS response, particularly any unexpected IP addresses.

### Alert Notifications

- When an alert is triggered, notifications are sent through all the channels configured on your account. These can include:
  - Email
  - Webhooks
  - Instant Messaging (IM) platforms like Slack, Teams, and Google Chat.

## Alert Closure

- An alert is automatically closed when the conditions set in the 'Number of Checks to Declare Monitor Up' are met. This means that the monitor must have a specified number of consecutive successful checks to consider the issue resolved.

## Summary

Alerts in mon1tor play a pivotal role in ensuring you are promptly informed about any disruptions or changes in your monitored services. By configuring alert thresholds and notification channels, you can maintain a proactive stance in managing and resolving issues.
