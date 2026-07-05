# Invalid Ticker Runbook

## Alert

Stock data could not be downloaded.

## Symptoms

- yfinance returns empty dataframe
- "No data found"
- Workflow stops at Data Agent

## Investigation

1. Check LangSmith trace.
2. Verify ticker symbol.
3. Confirm Yahoo Finance availability.
4. Check internet connectivity.

## Resolution

- Correct ticker symbol.
- Retry download.

## Escalation

Only if Yahoo Finance service is unavailable.
