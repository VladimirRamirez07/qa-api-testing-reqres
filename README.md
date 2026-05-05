# QA API Testing - ReqRes

Automated API testing project using Postman, Newman and GitHub Actions CI/CD.

## 🛠️ Tech Stack
- **Postman** - API test collection
- **Newman** - CLI test runner
- **GitHub Actions** - CI/CD pipeline

## 📋 Test Coverage
| Endpoint | Method | Tests |
|----------|--------|-------|
| /api/users | GET | Status, response time, data structure |
| /api/users/2 | GET | Status, user id, email format |
| /api/users | POST | Status 201, id, createdAt |
| /api/login | POST | Status 200, token |

## 🚀 Run locally
```bash
npm install -g newman newman-reporter-htmlextra
newman run collections/reqres-api-tests.postman_collection.json
```

## ✅ CI/CD
Every push to main triggers the test suite automatically via GitHub Actions.