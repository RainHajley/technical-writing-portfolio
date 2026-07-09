# Chat Completions API

Use the `/v1/chat/completions` endpoint to generate text or conversational responses.

## Endpoint

`POST https://nexus-ai.io`

## Authentication

Include your secret key in the request header:

```http
Authorization: Bearer <YOUR_NEXUS_API_KEY>
Content-Type: application/json
```

## Request Body

| Parameter | Type | Required | Description |
| :--- | :--- | :--- | :--- |
| `model` | string | **Yes** | `nexus-4-omni` or `nexus-4-turbo`. |
| `messages` | array | **Yes** | Conversation history (see below). |
| `temperature` | float | No | Randomness: `0.0` (deterministic) to `2.0` (creative). Default: `1.0`. |
| `max_tokens` | integer | No | Response limit. Default: `4096`. |

### The messages Object

Each object in the array requires:

* **role**: `system` (context), `user` (input), or `assistant` (AI output).
* **content**: The text payload.

## Example Request

```bash
curl https://nexus-ai.io \
  -H "Authorization: Bearer YOUR_NEXUS_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "nexus-4-turbo",
    "messages": [
      {"role": "system", "content": "You are a senior refactoring engineer."},
      {"role": "user", "content": "Refactor this function to remove nested loops."}
    ],
    "temperature": 0.2,
    "max_tokens": 512
  }'
```

## Response

A successful response (`200 OK`) returns a JSON object:

```json
{
  "id": "chatcmpl_8vX29KlnM27x",
  "model": "nexus-4-turbo",
  "choices": [{
    "message": {
      "role": "assistant",
      "content": "..."
    },
    "finish_reason": "stop"
  }],
  "usage": {
    "prompt_tokens": 42,
    "completion_tokens": 38,
    "total_tokens": 80
  }
}
```

## Troubleshooting

| Status | Error | Remediation |
| :--- | :--- | :--- |
| `400` | `invalid_payload` | Check JSON schema and required fields. |
| `401` | `invalid_api_key` | Verify your token in the header. |
| `429` | `rate_limit_exceeded` | Implement exponential backoff. |
