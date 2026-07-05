# Gemini API Failure

## Symptoms

- 401 Unauthorized
- 403 Forbidden
- 429 Too Many Requests

## Investigation

1. Open LangSmith trace.
2. Inspect Recommendation Agent.
3. Verify API Key.
4. Check Gemini quota.
5. Check Google AI status.

## Resolution

- Refresh API key.
- Retry request.
- Use backup model.

## Escalation

Platform Team
