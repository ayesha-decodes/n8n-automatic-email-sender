# n8n-automatic-email-sender

An automated cold email workflow. This workflow helps send personalized cold emails at scale using randomized templates.

## Features

- Fetches leads from Google Sheets
- Filters out already sent emails
- Uses multiple email templates
- Randomly selects a template for each lead
- Personalizes emails using lead names
- Sends emails automatically via Gmail
- Prevents duplicate outreach (with status tracking)

## Workflow Overview

```text
Manual Trigger
     ↓
Fetch Leads from Sheet1
     ↓
Check "Send Status"
     ↓
Loop Through Leads
     ↓
Fetch Templates from Sheet2
     ↓
Random Template Selection
     ↓
Merge Lead + Template
     ↓
Personalize Email
     ↓
Send via Gmail
