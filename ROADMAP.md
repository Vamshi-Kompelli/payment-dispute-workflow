# Build Roadmap

## Phase 1 - Python domain model
Create `PaymentDispute` with amount validation, valid statuses, allowed transitions, per-instance history, and undo.

## Phase 2 - Service layer
Create a manager/service that adds, finds, updates, filters, removes, counts, and summarizes disputes. Prevent duplicate dispute IDs.

## Phase 3 - REST API
Add FastAPI routes for create, retrieve, list, update status, and delete. Use Pydantic schemas and meaningful HTTP status codes.

## Phase 4 - Persistence
Replace in-memory storage with PostgreSQL and SQLAlchemy. Add Alembic migrations, constraints, timestamps, and indexes.

## Phase 5 - Security
Add password hashing, JWT access tokens, role-based permissions, and secrets through environment variables.

## Phase 6 - Quality
Add pytest unit/integration tests, test database isolation, structured logging, linting, and type checks.

## Phase 7 - Delivery
Add Dockerfile, Compose, health endpoint, GitHub Actions, and deployment notes.

## Phase 8 - AI extensions
Add classifier, structured document extraction, policy RAG, evaluation cases, confidence handling, human review, and audit logging. Never send real customer data to external AI services.
