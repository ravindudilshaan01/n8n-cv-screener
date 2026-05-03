# Automated CV Screening Workflow

n8n pipeline that fetches CV PDFs from Google Drive, 
scores them against a role using Gemini 2.5 Flash, 
and outputs structured results to Google Sheets.

## What it does
- Fetches PDFs from a specified Google Drive folder
- Sends each CV to Gemini with a structured scoring prompt
- Extracts: match score, key skills, summary
- Writes timestamped results to Google Sheets
- Handles rate limits (5s delay, 15 req/min)
- Duplicate-safe — won't re-process existing entries

## Tech
- n8n (self-hosted or cloud)
- Google Gemini 2.5 Flash Lite
- Google Drive API
- Google Sheets API

## How to import
1. Open n8n
2. New Workflow → Import from file
3. Select `List CV Uploads.json`
4. Add your Google credentials
5. Run

## Screenshot
[add a screenshot of the workflow canvas here]
