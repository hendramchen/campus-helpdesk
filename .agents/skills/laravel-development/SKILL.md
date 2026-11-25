---
name: laravel-development
description: Implement and modify Laravel application features using Laravel conventions, Eloquent, Form Requests, Policies, Blade, migrations, and automated tests. Use when creating controllers, models, routes, database changes, validation, authorization, or business operations in a Laravel project.
---

# Laravel Development Skill

## Objective

Implement maintainable Laravel features following
the project's architecture and requirements.

## Before Implementation

1. Read the relevant project documentation.
2. Inspect existing related models and controllers.
3. Identify existing naming conventions.
4. Check whether reusable functionality exists.
5. Identify authorization and validation requirements.

## Implementation Guidelines

### Controllers

- Keep controllers focused on HTTP coordination.
- Avoid implementing complex business logic directly.
- Use dependency injection when appropriate.

### Validation

- Use Form Request classes for feature-level
  request validation.
- Keep validation rules explicit.
- Return appropriate validation responses.

### Models

- Define Eloquent relationships.
- Protect mass assignment.
- Use appropriate casts.
- Avoid unnecessary model complexity.

### Business Logic

- Keep simple operations close to their
  appropriate Laravel components.
- Extract reusable orchestration into Actions
  or Services when justified.
- Avoid premature abstraction.

### Database

- Create migrations for schema changes.
- Add foreign keys and appropriate indexes.
- Use transactions when necessary.

### Authorization

- Use Policies or Gates where appropriate.
- Never rely only on hiding UI elements.
- Verify authorization on the server.

### Testing

- Write feature tests for HTTP behavior.
- Test validation and authorization.
- Test important business rules.

## Completion Checklist

- [ ] Requirements are satisfied.
- [ ] Code follows project conventions.
- [ ] Validation is implemented.
- [ ] Authorization is enforced.
- [ ] Database changes are correct.
- [ ] Relevant tests pass.
- [ ] No unrelated files were modified.
