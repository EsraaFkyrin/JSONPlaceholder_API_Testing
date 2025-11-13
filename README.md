# JSONPlaceholder API –  Testing Suite

>  Full CRUD + Negative Testing | **100% Pass Rate**
------------

## Overview

A **production-grade Postman collection** demonstrating **enterprise-level API testing practices** on the [JSONPlaceholder](https://jsonplaceholder.typicode.com) fake REST API.

This project covers:
- **Full CRUD operations** (Create, Read, Update, Delete)
- **Request chaining** using dynamic IDs
- **Positive & negative scenarios**
- **Automated validation** with `pm.test`
- **Console debugging** and **visual feedback**

---

## Key Features

| Feature | Description |
|-------|-----------|
| {{new_post_id}} | Dynamic ID injection across requests |
| Environment Variables | Configurable base URL & test data |
| 18+ Automated Tests | Status codes, JSON schema, data integrity |
| Pre-request Scripts | Fail-fast validation |
| Console Logging | Full debug visibility |
| PDF Execution Report | Professional test summary |

---

## Test Cases Summary

| # | Test Case | Method | Endpoint | Expected | Status |
|---|----------|--------|----------|----------|--------|
| 1 | Retrieve all posts | `GET` | `/posts` | 200 + 100 items | PASS |
| 2 | Create new post | `POST` | `/posts` | 201 + ID generated | PASS |
| 3 | Full update post | `PUT` | `/posts/:id` | 200 + full replace | PASS |
| 4 | Partial update | `PATCH` | `/posts/:id` | 200 + title only | PASS |
| 5 | Delete post | `DELETE` | `/posts/:id` | 200 + `{}` | PASS |
| 6 | Invalid ID | `GET` | `/posts/999999` | 404 + `{}` | PASS |

> **Total Tests: 18** | **Pass Rate: 100%** | **Execution Time: ~2.4s**

---

## Project Structure
JSONPlaceholder-API-Testing/
├── collection/
│   └── JSONPlaceholder_Professional.postman_collection.json
├── environment/
│   └── JSONPlaceholder_Env.postman_environment.json
├── reports/
│   └── API_Testing_Report_JSONPlaceholder.pdf
├── screenshots/
│   └── passed_tests.png
├── README.md
└── LICENSE


---

## How to Run

1. **Import** the collection and environment into Postman
2. **Select** `JSONPlaceholder Professional Env`
3. **Run requests in order**:
GET → POST → PUT → PATCH → DELETE → NEGATIVE
4. **Open Console** (`Ctrl+Alt+C`) to view logs
5. **Export PDF report** from Postman Runner

 ## Tools & Technologies

- **Postman** – v11 (Desktop)
- **REST API** – JSONPlaceholder
- **HTTP Methods** – GET, POST, PUT, PATCH, DELETE
- **JavaScript** – `pm.test`, `pm.globals`, `console.log`
- **Reporting** – PDF + Screenshots

    

   
