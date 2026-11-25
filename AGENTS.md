# Project Instructions

## 1. Project Context

This project is a Campus IT Helpdesk application
built using Laravel.

Before implementing any feature, understand the
requirements in the `docs/` directory.

Documentation is the source of truth for
business requirements and business rules.

Do not invent requirements or add features
without explicit approval.

## 2. Technology Stack

- Backend: Laravel
- Language: PHP
- Frontend: Laravel Blade
- Database: MySQL

Always inspect composer.json and the existing
project before assuming framework versions.

Prefer existing dependencies and Laravel's
built-in capabilities.

Do not install additional packages without
explaining why and requesting approval.

## 3. Architecture Guidelines

Follow Laravel conventions and maintain clear
separation of responsibilities.

Use:

- Controllers for HTTP request coordination.
- Form Requests for request validation.
- Eloquent Models for persistence and relationships.
- Policies or Gates for authorization.
- Services or Actions when business operations
  require reusable orchestration.
- Blade for presentation.
- Database migrations for schema changes.

Avoid unnecessary abstraction.

Do not introduce repositories, interfaces,
DTOs, or complex DDD structures unless there
is a clear requirement.

## 4. Coding Standards

- Follow PSR-12.
- Use meaningful class and method names.
- Prefer dependency injection.
- Avoid duplicated business logic.
- Keep controllers focused.
- Avoid massive models and controllers.
- Use database transactions when an operation
  requires atomic changes.
- Handle exceptions appropriately.
- Never hardcode secrets or credentials.

## 5. Database Guidelines

- Use Laravel migrations.
- Define foreign keys and appropriate indexes.
- Use Eloquent relationships.
- Avoid unnecessary database queries.
- Prevent N+1 query problems.
- Never modify production data.
- Do not run destructive database commands
  without explicit approval.

## 6. Security Guidelines

- Validate all user input.
- Enforce authorization on protected actions.
- Protect against mass assignment.
- Use CSRF protection.
- Never expose sensitive information.
- Never commit .env or credentials.
- Ensure users cannot access tickets they
  are not authorized to view.

## 7. Testing Guidelines

- Write tests for business-critical behavior.
- Test authorization and validation.
- Test database relationships.
- Test important success and failure scenarios.
- Run relevant tests after implementation.

Never claim tests passed without executing them.

## 8. Development Workflow

For every feature:

1. Understand the requirement.
2. Inspect the existing implementation.
3. Identify affected files and components.
4. Analyze possible side effects.
5. Present an implementation plan.
6. Wait for approval before implementation
   when the task requests planning or approval.
7. Implement incrementally.
8. Run relevant tests.
9. Review the changes.
10. Summarize what was implemented.

## 9. Git Guidelines

- Do not overwrite unrelated changes.
- Do not reset or discard user changes.
- Do not commit unless explicitly requested.
- Keep changes focused on the requested task.

## 10. Communication

Before making significant architectural decisions,
explain the trade-offs.

Ask questions when business requirements
are ambiguous.

Clearly distinguish:

- Existing implementation
- Confirmed requirements
- Assumptions
- Proposed improvements
