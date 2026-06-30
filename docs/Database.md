# Database Design

## Overview

CloudCodeMentor uses Microsoft Azure SQL Database as its primary relational database.

The database is designed to support multiple users, multiple projects per user, code analysis history, AI-generated suggestions, and future platform expansion.

---

# Why Azure SQL Database?

The project requires a relational database because the data contains strong relationships between entities.

Examples include:

- One user can own multiple projects.
- One project can contain multiple code analyses.
- One analysis can generate multiple suggestions.

Azure SQL Database provides:

- Reliability
- Scalability
- Security
- High availability
- Integration with Azure services

---

# Planned Database Structure

## Users

Stores user accounts.

Fields

- UserId
- FullName
- Email
- PasswordHash
- Role
- CreatedAt

---

## Projects

Stores programming projects created by users.

Fields

- ProjectId
- UserId
- ProjectName
- ProgrammingLanguage
- CreatedAt

---

## CodeAnalysis

Stores every code analysis performed by the platform.

Fields

- AnalysisId
- ProjectId
- OriginalCode
- ImprovedCode
- Explanation
- Score
- CreatedAt

---

## Suggestions

Stores AI-generated recommendations.

Fields

- SuggestionId
- AnalysisId
- Type
- Description

---

## ActivityLog

Stores important user activities.

Fields

- LogId
- UserId
- Action
- Timestamp

---

# Entity Relationships

Users

↓

Projects

↓

CodeAnalysis

↓

Suggestions

Users

↓

ActivityLog

---

# Future Expansion

The database is designed to support future features without major structural changes.

Planned future additions include:

- Team collaboration
- GitHub repositories
- Code versions
- Notifications
- AI history
- File uploads

---

# Current Status

Sprint 1

Database architecture designed.

Sprint 2

Database implementation will begin.