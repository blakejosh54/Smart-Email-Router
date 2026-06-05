# Smart Email Router

This is an n8n automation workflow that sorts incoming Gmail emails into different categories and logs the result.

The workflow checks incoming emails, routes them through different branches, applies Gmail labels, sends a Slack notification for lead-related emails, and appends the processed email details to a Google Sheet.

## Tools Used

- n8n
- Docker
- Gmail
- Slack
- Google Sheets

## What It Does

- Triggers when a new Gmail email comes in
- Uses switch logic to classify emails as:
  - Invoice
  - Lead
  - Urgent
  - Other
- Adds Gmail labels based on the email type
- Sends a Slack message for lead emails
- Logs processed emails into Google Sheets

## Notes

This repository does not include any credentials, API keys, or private tokens. Anyone importing the workflow will need to connect their own Gmail, Slack, and Google Sheets accounts.