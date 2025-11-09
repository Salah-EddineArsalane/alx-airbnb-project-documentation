# Airbnb Clone – Backend Requirement Specifications

## Overview
This document defines the **functional and technical requirements** for the main backend features of the Airbnb Clone project.  
Each section describes expected behaviors, API endpoints, request/response formats, validation rules, and performance considerations.

---

## 1. User Authentication System

### **Functional Requirements**
- Users must be able to register, log in, and log out.
- Passwords must be securely stored using hashing (e.g., bcrypt).
- Authentication tokens (JWT) should be used for session management.
- Invalid credentials should return appropriate error messages.

### **API Endpoints**
| Method | Endpoint | Description | Authentication |
|--------|-----------|--------------|----------------|
| `POST` | `/api/auth/register` | Register a new user | No |
| `POST` | `/api/auth/login` | Log in a user | No |
| `GET` | `/api/auth/profile` | Retrieve user info | Yes |

### **Request and Response Examples**

#### ➤ Register
**Input:**
```json
{
  "name": "John Doe",
  "email": "john@example.com",
  "password": "SecurePass123"
}
