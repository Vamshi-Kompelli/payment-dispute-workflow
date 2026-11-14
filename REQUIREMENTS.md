# Functional Requirements

## Dispute fields
- dispute_id: unique string
- transaction_id: string
- amount: decimal greater than zero
- reason: non-empty string
- status: OPEN by default
- created_at and updated_at

## Allowed transitions
- OPEN -> UNDER_REVIEW
- UNDER_REVIEW -> RESOLVED
- UNDER_REVIEW -> REJECTED
- RESOLVED and REJECTED are terminal

## Required API behavior
- Create, retrieve, list, update status, and delete disputes
- Filter by status and amount range
- Paginate list responses
- Return consistent validation errors
- Record status history and actor
- Protect write operations with authentication

## Definition of done
- Tests cover success, invalid input, duplicate IDs, missing records, invalid transitions, terminal states, and empty collections
- README contains setup and API examples
- No secrets or real banking/customer data in Git history
