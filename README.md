# Cooperative Banking Platform

A production-ready cooperative banking and micro-finance management system built with Laravel and Flutter. Designed for cooperative societies to digitize their operations from branch management to field collections.

## 🏗️ Architecture

The platform follows a clean three-tier architecture:

- **Client Layer**: Cross-platform Flutter app (Android/Web) with role-based UI and offline-first data sync
- **API Layer**: Laravel RESTful API with token-based authentication and role-scoped access control
- **Data Layer**: Relational database with ledger-based financial transactions and comprehensive audit trails

## 🎯 Core Features

### Role-Based Access Control
- **Super Admin**: System-wide configuration and oversight
- **Admin**: Multi-branch management and user provisioning
- **Manager**: Branch operations and approval workflows
- **Field Executive**: Customer onboarding and field collections
- **Customer**: Self-service portal for account management

### Financial Operations
- Multi-type account management (Savings, DD, RD, FD)
- Loan processing with approval workflows
- Field collection with offline sync capability
- Ledger-first transaction recording
- Receipt generation and document management

### Operational Features
- Branch hierarchy and staff management
- KYC document handling
- Role-scoped dashboards and analytics
- Report generation and exports
- Audit logging and session management

## 🛠️ Technology Stack

**Backend**
- Laravel (PHP framework)
- RESTful API design
- Token-based authentication
- MySQL/MariaDB database
- cPanel-compatible deployment

**Frontend**
- Flutter framework
- Cross-platform (Android/Web)
- Offline-first architecture
- SharedPreferences for local storage

**Key Services**
- Session management with token expiry
- OTP verification (Email/SMS)
- PDF generation for receipts
- Scheduled financial tasks
- Activity logging and auditing

## 📐 System Design

The system implements several key architectural patterns:

1. **Service Layer Pattern**: Business logic encapsulated in dedicated service classes
2. **Repository Pattern**: Data access abstraction through Eloquent models
3. **Middleware Pipeline**: Request validation, authentication, authorization, and logging
4. **Role-Based Access Control**: Fine-grained permissions based on user roles and hierarchy
5. **Ledger-First Accounting**: All financial transactions recorded with double-entry principles

## 🔐 Security Features

- Token-based API authentication
- Role and permission-based authorization
- Rate limiting on sensitive endpoints
- Activity logging for audit trails
- Secure session management with expiry
- Input validation and sanitization

## 🚀 Deployment

Optimized for shared hosting environments:
- Single codebase deployment
- cPanel-compatible structure
- Environment-based configuration
- Database migration system
- Scheduled task automation

## 📊 Data Flow

Client Request 
→ Rate Limiting → Token Auth → Role Check → Controller
→ Service Layer → Ledger Validation → Database → Response
→ Activity Log → Client

## 🏢 Use Cases

Ideal for:
- Cooperative credit societies
- Micro-finance institutions
- Community banking operations
- Small to medium-sized lending organizations
- Organizations requiring field collection capabilities
