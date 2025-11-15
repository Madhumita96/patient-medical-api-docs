Retrieve a single patient's detailed information.

---

## Path Parameter

| Parameter | Type | Required | Description |
|----------|------|----------|-------------|
| id | integer | Yes | Unique patient ID |

---

## Example Request

```bash
curl -X GET "https://api.example.com/v1/api/patients/101" \
-H "Authorization: Bearer YOUR_API_KEY"
```
## Success Response (200 OK)
```
{
  "id": 101,
  "name": "John Doe",
  "age": 45,
  "gender": "Male",
  "diagnosis": "Hypertension"
}
```
## Error Responses

404 Not Found
```
{ "error": "Patient not found" }

```
