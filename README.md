# user-management-api-test-suite

Repository ini berisi dokumentasi dan artefak pengujian API untuk fitur Authentication, Users, dan Resources menggunakan Reqres sebagai System Under Test (SUT).

Fokus pengujian adalah memastikan endpoint dapat merespons request dengan benar, menangani error secara konsisten, serta mengembalikan data sesuai contract yang diharapkan.

---

## Test Scope

### Authentication

Test scenario yang diuji:

- Valid Login
- Invalid Credentials
- Missing Email
- Missing Password
- Empty Request Body
- Response Validation
- Response Time Validation

Total Test Cases: 9

---

### Users

Test scenario yang diuji:

- List Users
- Single User
- User Not Found
- Create User
- Update User
- Partial Update User
- Delete User
- Pagination Validation
- Negative Testing

Total Test Cases: 13

---

### Resources

Test scenario yang diuji:

- List Resources
- Single Resource
- Resource Not Found
- Schema Validation
- Response Time Validation

Total Test Cases: 4

---

## Testing Approach

Pengujian dilakukan menggunakan pendekatan:

- Functional Testing
- Positive Testing
- Negative Testing
- Boundary Testing
- Response Validation
- Status Code Validation
- Schema Validation
- Response Time Validation

---

## Automation

Automation dibuat menggunakan Postman Collection dan JavaScript Assertion.

Implementasi yang digunakan:

- Environment Variables
- Automated Assertions
- Collection Organization
- Response Validation
- JSON Schema Validation

---

## Project Structure

```text
user-management-api-test-suite/

├── collections/
│   └── user-management-api.postman_collection.json

├── environments/
│   └── reqres-environment.postman_environment.json

├── docs/
│   └── test-cases.md

└── README.md
```

---

## Tools

- Postman
- Newman
- JavaScript
- GitHub

---

## Execution

Collection dapat dijalankan melalui:

### Postman Collection Runner

atau menggunakan Newman:

```bash
newman run user-management-api.postman_collection.json
```

---

## Test Result Summary

| Module | Total Test Cases |
|----------|----------:|
| Authentication | 9 |
| Users | 13 |
| Resources | 4 |
| Total | 26 |

Seluruh test case berhasil dieksekusi sesuai expected result.

---

## Catatan

Project ini dibuat sebagai bagian dari QA API Testing Portfolio dengan fokus pada automation testing menggunakan Postman.

System Under Test menggunakan public API dari Reqres untuk mensimulasikan skenario pengujian Authentication, Users, dan Resources.
