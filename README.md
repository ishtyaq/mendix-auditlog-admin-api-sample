# Mendix Audit Log Admin API – Sample App

This repository contains a minimal Mendix sample application that demonstrates
how to dynamically control Mendix runtime log levels using the Admin API.

It is a companion project for the article:
<a href="https://www.linkedin.com/pulse/how-hidden-mendix-api-fixed-my-auditlogs-ishtiaq-ahmad-ovebf/"> **"How a Hidden Mendix API Fixed My Audit Logs"** </a>

<img width="1842" height="697" alt="image" src="https://github.com/user-attachments/assets/7799517f-7b8c-41db-bddf-4c0a56f63bc7" />


## What this sample shows
- Verifying access to the Mendix Admin service port
- Updating log levels (Trace, Debug, Info, Warning, Error) at runtime
- Verifying log output by triggering real database transactions
- Safe usage guidance for TRACE logs in production-like environments

## Prerequisites
- Mendix Studio Pro 10.x
- Access to the Mendix Admin service port. Only available for on-premise/local. Admin API is restricted on cloud. 
- Admin password configured in Runtime Advanced Settings

## How to use
1. Open the project in Mendix Studio Pro
2. Verify the Admin service port and credentials
3. Use the UI to update runtime log levels
4. Trigger sample actions to verify log output

## Notes
- TRACE logs can generate large volumes of data
- Log files are rolled over but not automatically deleted on Windows/on-prem
- Enable TRACE only for short diagnostic windows

## Disclaimer
This is a sample application intended for learning and troubleshooting purposes.
Use appropriate security and operational controls before applying in production.
