---
title: Close Alert  
nextjs:
  metadata:
    title: 'How to Close Alerts in mon1tor - User Guide'
    description: 'Discover how to manually or automatically close alerts in mon1tor and understand how it affects your monitor's status.'
---


Understanding how alerts are closed is an essential aspect of managing your monitoring with mon1tor. Alerts can be closed automatically or manually, each method influencing the subsequent monitoring behavior differently. This guide explains both automatic and manual closure of alerts.

## Automatic Alert Closure

An alert is automatically closed in mon1tor under the following condition:

- **Recovery Confirmation**: When the number of consecutive successful checks meets the threshold set in 'Number of Checks to Declare Monitor Up', the alert is automatically closed. This indicates that the monitored service has returned to its expected state of operation.

## Manual Alert Closure

You also have the option to manually close an alert:

- **Manual Intervention**: Users can close an alert manually at any time. This action will stop the sending of further notifications and will reset the monitor's expected conditions based on the most recent data received.

    - For a **Code HTTP Monitor**: If an alert was raised due to an unexpected HTTP code (e.g., 400 instead of 200) and you manually close the alert, the new expected code for future checks will be updated to the most recent one received (in this case, 400).
  
    - For a **DNS Monitor**: Similarly, if an alert was triggered due to unexpected IP changes, manually closing the alert will set the new IPs received as the expected ones for future monitoring.

### Considerations for Manual Closure

- **Impact on Monitoring**: Manually closing an alert redefines what is considered 'normal' for the monitor. It's important to understand that this action adjusts the monitor's baseline for future alerts.
  
- **Use with Caution**: Manual closure should be used judiciously, especially in situations where the change in response (HTTP code or DNS IP) is temporary or not indicative of a new normal state.

## Summary

Alert closure, whether automatic or manual, is a significant function in mon1tor's alert management system. Automatic closure ensures a return to normal operation, while manual closure offers flexibility in handling anomalies and redefining what is considered normal for your monitoring needs.

