# API Documentation Template

This template provides guidelines for documenting all NexaFlow APIs.

## 📡 API Overview

All NexaFlow APIs follow REST principles and return JSON responses.

**Base URL:** `https://api.nexaflow.com/v1`

## 🔐 Authentication

All API requests require authentication using Bearer tokens:
```http
Authorization: Bearer YOUR_API_TOKEN
```

## 📋 Standard Response Format

### Success Response
```json
{
  "success": true,
  "data": {
    // Response payload
  },
  "meta": {
    "timestamp": "2024-01-15T10:30:00Z"
  }
}
```

### Error Response
```json
{
  "success": false,
  "error": {
    "code": "INVALID_REQUEST",
    "message": "Detailed error message"
  }
}
```

## 🚀 Example Endpoint Documentation

### GET /users/:id

Retrieve user details by ID.

**Parameters:**
- `id` (path, required) - User identifier

**Response:** `200 OK`
```json
{
  "success": true,
  "data": {
    "id": "usr_123",
    "name": "John Doe",
    "email": "john@example.com"
  }
}
```

## 📊 Rate Limiting

- **Standard tier:** 100 requests per minute
- **Premium tier:** 1000 requests per minute

## 🛠️ Best Practices

1. Always include error handling
2. Use appropriate HTTP status codes
3. Version your APIs (e.g., /v1, /v2)
4. Document all breaking changes

---

**Maintained by:** Backend Team | **Last updated:** 2024
```

---

### **Expected Output:**

After `git pull origin main`:
```
Already up to date.
```
*(Since main hasn't changed yet)*

After `git branch`:
```
* feature/api-documentation-template
  main
```

After `git push`:
```
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to X threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), [size], done.
Total 4 (delta 0), reused 0 (delta 0)
remote:
remote: Create a pull request for 'feature/api-documentation-template' on GitHub by visiting:
remote:      https://github.com/YOUR_USERNAME/nexaflow-docs/pull/new/feature/api-documentation-template
remote:
To https://github.com/YOUR_USERNAME/nexaflow-docs.git
 * [new branch]      feature/api-documentation-template -> feature/api-documentation-template
Branch 'feature/api-documentation-template' set up to track remote branch 'feature/api-documentation-template' from 'origin'.