# Authentication

The Patient Medical Data API uses **API Key–based Bearer Token authentication**.

Every request must include the following header:

---

**Authorization**: Bearer YOUR_API_KEY



## How It Works

1. You obtain an API key from the system administrator.
2. You include the API key in the **Authorization** header.
3. If the key is valid, the API will process your request.
4. If not, you receive a `401 Unauthorized` error.

---

## Example cURL Request

```bash
curl -X GET "https://api.example.com/v1/api/patients" \
-H "Authorization: Bearer YOUR_API_KEY"
---
| Status Code               | Meaning             | Description                      |
| ------------------------- | ------------------- | -------------------------------- |
| **401 Unauthorized**      | Invalid API Key     | Token is missing or incorrect    |
| **403 Forbidden**         | Not allowed         | API key does not have permission |
| **429 Too Many Requests** | Rate limit exceeded | Too many requests in short time  |
