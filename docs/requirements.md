# Requirements Engineering Specification

## 1. Functional Requirements Specification (FRS)

### FR-01 — Authentication

The platform shall provide secure Role-Based Access Control (RBAC) for:

- Admin
- Librarian
- Student
- Faculty

### FR-02 — Book Catalog Management

The platform shall support full CRUD operations for:

- Books
- Authors
- Categories
- Physical shelf coordinates

### FR-03 — Circulation Engine

The platform shall support automated:

- Check-out processing
- Check-in processing
- Inventory increment/decrement

### FR-04 — Fine Engine

The platform shall provide automated background processing for calculating overdue penalties based on user tier.

### FR-05 — Notification System

The platform shall trigger email alerts for:

- Upcoming due dates
- Overdue fines

---

# 2. Non-Functional Requirements Specification (NFRS)

### NFR-01 — Security

The platform shall support:

- Password hashing using Bcrypt/Argon2
- JWT token session management
- HTTPS encryption

### NFR-02 — Performance

The platform shall target sub-500ms API response time for search queries under concurrent user load.

### NFR-03 — Availability & Scalability

The platform shall target 99.9% uptime using containerized deployment and horizontal pod autoscaling.

### NFR-04 — Maintainability

The platform shall use Infrastructure as Code (IaC) modularity and clear codebase separation.