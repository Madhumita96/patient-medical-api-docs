## API endpoint overview

This section provides a high-level summary of all available API endpoints.  
Detailed documentation for each endpoint exists in the **endpoints/** folder.

---

## Patient Endpoints

| Method | Endpoint | Description | Detailed Doc |
|--------|----------|-------------|--------------|
| **GET** | `/api/patients` | List all patients | [get-patients.md](../endpoints/get-patients.md) |
| **GET** | `/api/patients/{id}` | Get patient by ID | [get-patient-by-id.md](../endpoints/get-patient-by-id.md) |
| **POST** | `/api/patients` | Create new patient | [post-patient.md](../endpoints/post-patient.md) |
| **PUT** | `/api/patients/{id}` | Update patient record | [put-patient.md](../endpoints/put-patient.md) |
| **DELETE** | `/api/patients/{id}` | Delete patient record | [delete-patient.md](../endpoints/delete-patient.md) |

---

## Response Format
All responses are in JSON format.

---

## Status Codes

| Code | Meaning |
|------|---------|
| 200 | Success |
| 201 | Record created |
| 400 | Bad request |
| 401 | Unauthorized |
| 404 | Not found |
| 500 | Server error |

---

For detailed usage, open the endpoint files inside the **endpoints/** folder.
