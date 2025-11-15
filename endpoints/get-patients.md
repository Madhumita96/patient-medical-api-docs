# GET /api/patients

Retrieve a paginated list of all patients.

---

## Request

### Query Parameters
| Parameter | Type | Required | Description |
|----------|------|----------|-------------|
| page | integer | No | Page number (default: 1) |
| limit | integer | No | Records per page (default: 10) |

---

## Example request

```bash
curl -X GET "https://api.example.com/v1/api/patients?page=1&limit=10" \
-H "Authorization: Bearer YOUR_API_KEY"
```
## Success response (200 OK)
```
{
  "page": 1,
  "limit": 10,
  "total_records": 120,
  "patients": [
    {
      "id": 101,
      "name": "John Doe",
      "age": 45,
      "gender": "Male",
      "diagnosis": "Hypertension"
    }
  ]
}
```
---
## Error response 
### 400 Bad Request
```
{ "error": "Invalid page number" }
```
### 401 Unauthorized
```
{ "error": "Missing or invalid token" }

```
