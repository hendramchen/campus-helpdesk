# Campus Helpdesk

A ticketing system for campus IT support. Lecturers and employees report problems; admins triage and assign; IT staff resolve.

## Features (MVP)

- Create tickets with title, description, priority
- Role-based access: **Requester** (lecturer/employee), **Admin**, **IT Staff**
- Admin assigns tickets to IT staff
- Status workflow: `open` → `in_progress` → `closed`
- Comments and an activity log per ticket
- Filter and search by status, priority, assignee

## Tech stack

Laravel 12 · PHP 8.3+ · MySQL/PostgreSQL · Blade + Livewire · Tailwind CSS · Pest

## Getting started

```bash
git clone <repo-url> campus-helpdesk && cd campus-helpdesk
composer install
cp .env.example .env
php artisan key:generate
# set DB_* in .env, then:
php artisan migrate --seed
npm install && npm run dev
php artisan serve
```

Seeded demo accounts (local only, password `password`):

| Role      | Email                |
| --------- | -------------------- |
| Admin     | admin@campus.test    |
| IT Staff  | staff@campus.test    |
| Requester | lecturer@campus.test |

## Quality checks

```bash
composer check   # pint + larastan + pest
```

## Documentation

| Doc                                                            | Purpose                                    |
| -------------------------------------------------------------- | ------------------------------------------ |
| [00 Project overview](docs/00-project-overview.md)             | Goals, scope, users                        |
| [01 Business requirements](docs/01-business-requirements.md)   | Functional and non-functional requirements |
| [02 Business rules](docs/02-business-rules.md)                 | Roles, permissions, workflow               |
| [03 Database design](docs/03-database-design.md)               | Tables, columns, indexes                   |
| [04 Architecture](docs/04-architecture.md)                     | Layers and folder conventions              |
| [05 Development guidelines](docs/05-development-guidelines.md) | Standards, testing, git                    |
| [06 Development roadmap](docs/06-development-roadmap.md)       | Phased plan                                |

## Working with AI agents

See [AGENTS.md](AGENTS.md) and `.agents/skills/` for agent instructions and playbooks.
