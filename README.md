# Aveniq
### Digital Product Ownership & Lifecycle Platform

**Every product has a story. Keep it connected.**

Aveniq is a digital product ownership and lifecycle management platform designed to maintain a product's identity and history throughout its lifetime.

It provides a centralized system for managing product purchases, invoices, warranties, return policies, service records and ownership transfers.

Each registered product receives a unique digital identity through a QR-based product passport, allowing its permitted lifecycle information to be accessed through a public interface.

## Problem Statement

Product-related information is often scattered across physical invoices, emails, warranty cards and service-center records. When ownership changes, important documents and maintenance history can become difficult to preserve.

Aveniq aims to solve this problem by providing a centralized, structured and secure platform for product ownership and lifecycle records.

## Core Features

- **Product Registration:** Register electronic products and generate unique digital identities.
- **Digital Product Passport:** Access permitted product information through a unique QR code.
- **Document Management:** Securely store invoices, warranty documents and repair evidence.
- **Warranty & Return Tracking:** Manage warranty periods, return deadlines and reminders.
- **Service History:** Maintain owner-reported, document-supported and provider-verified service records.
- **Service Provider Management:** Register, review and approve service providers.
- **Ownership Transfer:** Transfer product ownership securely while preserving historical records.
- **Notifications:** Generate reminders and important lifecycle notifications.
- **Administration & Auditing:** Manage providers, disputes and important platform activities.

## Technology Stack

| Layer | Technology |
|---|---|
| Backend | Java, Spring Boot |
| API | Spring Web, REST |
| Security | Spring Security, JWT |
| ORM | Spring Data JPA, Hibernate |
| Database | PostgreSQL |
| Caching | Redis |
| Build Tool | Maven |
| Database Migrations | Flyway |
| Testing | JUnit, Mockito |
| API Documentation | OpenAPI / Swagger |
| Containerization | Docker |
| Version Control | Git, GitHub |

*The stack will be implemented incrementally as development progresses.*

## Architecture

Aveniq follows a modular monolith architecture.

The application is organized into independent business modules within a single Spring Boot application.

Planned modules:

- Identity and Access Management
- Product Management
- Document Management
- Warranty and Return Management
- Service History and Verification
- Service Provider Management
- Digital Product Passport
- Ownership Transfer
- Notifications
- Administration and Audit

PostgreSQL serves as the primary source of truth. Redis is planned as a supporting cache rather than a replacement for persistent database records.

## Important Design Principles

- A QR code identifies a product; it does not independently prove ownership.
- Private documents and account information must never be exposed through public product pages.
- Missing service records must not be interpreted as proof that a product has never been repaired.
- Service verification levels must reflect the actual source and evidence of a record.
- Ownership transfers must preserve historical records and maintain transactional consistency.
- Sensitive operations must enforce both role-based and resource-level authorization.

## Project Documentation

| Document | Description |
|---|---|
| [Requirements](docs/requirements.md) | Functional and non-functional requirements |
| [Architecture](docs/architecture.md) | System architecture and module responsibilities |
| [ER Diagram](docs/er-diagram.md) | Database entities and relationships |
| [Database Design](docs/database-design.md) | PostgreSQL schema and design decisions |

## Development Roadmap

- [x] Requirements analysis and system design
- [x] Initial database design and ER modeling
- [ ] GitHub repository and documentation foundation
- [ ] Spring Boot project setup
- [ ] Authentication and authorization
- [ ] Product management
- [ ] Document management
- [ ] Warranty and return management
- [ ] Service history and verification
- [ ] Ownership transfer
- [ ] Notifications and background processing
- [ ] Testing and quality assurance
- [ ] Dockerization and deployment

## Project Status

**Current stage:** System design and repository initialization.

The implementation will be developed incrementally, with emphasis on clean architecture, database integrity, secure API design, transaction management and production-oriented backend engineering.

## License

All rights reserved.

This repository is publicly available for viewing and evaluation. No license is granted for copying, modifying, distributing or commercially using the source code without prior written permission from the copyright holder.