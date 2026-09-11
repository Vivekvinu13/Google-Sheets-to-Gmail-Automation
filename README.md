# n8n Google Sheets to Gmail Automation

## 📌 Project Overview

This n8n automation processes student data, applies business rules, structures personalized email content, validates email addresses, and sends welcome emails through Gmail.

The workflow is designed as part of the CAIE Course Program — Assignment 9: n8n Automation: Google Sheets to Gmail.

## 🎯 Assignment Objective

The assignment requires an n8n workflow that:

1. Starts the workflow.
2. Reads rows from a Google Sheet.
3. Structures the data into a clear email subject and message body.
4. Sends the email through Gmail.
5. Avoids sending emails to invalid or missing email addresses.
6. Handles empty data gracefully.

The assignment requires the following core nodes:

- Manual Trigger or Schedule Trigger
- Google Sheets (Get Rows)
- Edit Fields / Set or Code Node
- Gmail (Send Message)

## 🔄 Current Workflow

```text
On Form Submission
        ↓
Extract from File1
        ↓
Switch
        ↓
Basic LLM Chain1
        ↓
Loop Over Items
        ↓
Code in JavaScript1
        ↓
Switch
        ↓
IF
        ↓
Switch1
        ↓
Send Welcome Email
