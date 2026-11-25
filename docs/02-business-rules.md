# Business Rules

## Ticket Rules

1. Every ticket must belong to a user.
2. Every ticket must belong to a category.
3. Every ticket must have a subject.
4. Every ticket must have a description.

## Priority Rules

Allowed values:

- low
- medium
- high

## Status Rules

Allowed values:

- open
- in_progress
- resolved

## Authorization Rules

1. Students can create tickets.
2. Students can view their own tickets.
3. IT support staff can view tickets.
4. IT support staff can update ticket statuses.

## Data Integrity

1. A ticket cannot reference a nonexistent user.
2. A ticket cannot reference a nonexistent category.
3. Ticket status must use an allowed value.
4. Ticket priority must use an allowed value.
