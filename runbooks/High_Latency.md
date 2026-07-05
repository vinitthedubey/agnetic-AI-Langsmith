# High Latency

## Symptoms

Workflow execution exceeds 15 seconds.

## Investigation

1. Check LangSmith latency.
2. Identify slowest agent.
3. Verify Gemini response time.
4. Verify yfinance response time.

## Resolution

Retry request.

Reduce prompt size.

Enable caching.
