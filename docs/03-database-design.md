# Database Design

## Users

- id
- name
- email
- password
- role
- timestamps

## Categories

- id
- name
- description
- timestamps

## Tickets

- id
- user_id
- category_id
- subject
- description
- priority
- status
- timestamps

## Relationships

- User hasMany Tickets
- Ticket belongsTo User
- Category hasMany Tickets
- Ticket belongsTo Category
