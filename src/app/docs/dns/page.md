---
title: DNS Monitor  
nextjs:
  metadata:
    title: DNS Monitoring with mon1tor - Configuration Guide
    description: Ensure your DNS's health with mon1tor's DNS Monitor. Learn how to track hostname changes against expected IP addresses.
---


The DNS Monitor in mon1tor is designed to ensure the integrity and performance of your DNS records. It allows you to monitor specific hostnames against expected IP addresses and quickly alerts you to any discrepancies or changes. Below is a guide on configuring a DNS Monitor with the available settings.

## Configuration Options

### Basic Settings

1. **Name**: Provide a descriptive name for your DNS monitor for easy identification.

2. **Hostname**: Enter the hostname (e.g., example.com) you wish to monitor.

3. **IPs**: List the expected IP addresses for the given hostname. The monitor will check if the actual IP addresses resolved match these expected values.

### Monitoring Settings

1. **Number of Checks to Declare Monitor Down**: Define the count of consecutive checks that need to fail (when the resolved IP does not match the expected IPs) before the monitor is declared 'down'.

2. **Number of Checks to Declare Monitor Up**: Specify how many consecutive successful checks (where resolved IPs match the expected IPs) are required to change the monitor's status to 'up'.

3. **Interval**: Set the frequency at which the DNS checks are performed.

## Setting Up a DNS Monitor

1. **Access the 'Create Monitor' section** in your mon1tor dashboard.

2. **Input the Basic Settings**: Fill in the name, hostname, and the expected IPs.

3. **Configure the Monitoring Settings**: Set the number of checks for the monitor's 'down' and 'up' status and the interval for checks.

4. **Activate the monitor**. Your DNS Monitor is now operational, continuously verifying the DNS records against your specified parameters.

This DNS Monitoring tool is crucial for maintaining the reliability of your domain's DNS configuration and ensuring that your services remain accessible and secure.

