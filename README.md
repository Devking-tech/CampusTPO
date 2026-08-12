# CampusTPO

A lightweight foundation for building secure, authenticated web applications.

[CampusTPO](https://campustpo.com/) is built around a simple architecture that prioritizes maintainability, security, and low infrastructure overhead.

## Architecture

The application uses:

* Bun
* SQLite
* Server-rendered pages
* Modular repository/service architecture
* Authentication and session management

The goal is to avoid unnecessary infrastructure while keeping the application structured enough to evolve as requirements grow.

## Authentication

Authentication is treated as a core part of the application rather than an additional feature.

The foundation includes:

* Email/password authentication
* Email verification
* Google sign-in
* Password recovery
* Session management
* Account management

## Security

Security controls are incorporated throughout the application, including:

* Role-based access control
* CSRF protection
* Content Security Policy
* Rate limiting
* Password hashing
* Audit trails

## Architecture

A simplified representation of the application is:

```text
Routes
  ↓
Services
  ↓
Repositories
  ↓
SQLite
```

Keeping these responsibilities separated makes the codebase easier to understand, test, and extend.

## Why SQLite?

Not every application needs a separate database server from day one.

SQLite provides a simple database layer without requiring additional database infrastructure. Combined with WAL mode, it provides a practical starting point for applications where keeping deployment and operational complexity low is important.

Additional infrastructure can be introduced later when actual requirements justify it.

## Philosophy

CampusTPO follows a simple principle:

> Start with a focused, secure architecture and add complexity when the product actually needs it.

The objective isn't to build the biggest possible stack. It's to build a foundation that is easy to understand, maintain, deploy, and evolve.

Learn more at [campustpo.com](https://campustpo.com/).
# CampusTPO
