# Azure Resources

## Overview

CloudCodeMentor is built entirely on Microsoft Azure.

This document describes all Azure resources used throughout the project and their purpose.

---

# Azure Subscription

Subscription Type

- Azure Personal Subscription

Environment

- Development

Cloud Provider

- Microsoft Azure

---

# Resource Group

Name

rg-cloudcodementor-dev

Purpose

Acts as the main logical container for all Azure resources related to the development environment.

Status

 Active

---

# Storage Account

Name

stcloudcodementordev

Purpose

Provides cloud storage services for the application.

Future usage

- File uploads
- Generated reports
- Temporary storage
- Application assets

Status

 Active

---

# App Service Plan

Name

asp-cloudcodementor-dev

Operating System

Windows

Pricing Tier

Free (F1)

Purpose

Hosts the CloudCodeMentor Web Application.

Status

 Active

---

# Web App

Name

app-cloudcodementor-dev

Runtime

.NET 8

Purpose

Hosts the frontend application and public website.

Status

 Active

---

# Azure SQL Server

Name

sql-cloudcodementor-dev

Purpose

Hosts Azure SQL Databases for CloudCodeMentor.

Status

 Active

---

# Azure SQL Database

Name

sqldb-cloudcodementor-dev

Purpose

Stores application data.

Expected data

- Users
- Projects
- Code Analysis
- Suggestions
- History

Status

 Active

---

# Planned Azure Resources

The following Azure resources will be added in future sprints.

- Azure Functions
- Azure Key Vault
- Azure Blob Containers
- Application Insights
- Azure Monitor
- Azure AI Services

---

# Azure Resource Naming Convention

| Resource | Prefix |
|----------|---------|
| Resource Group | rg- |
| Storage Account | st |
| App Service Plan | asp- |
| Web App | app- |
| SQL Server | sql- |
| SQL Database | sqldb- |
| Function App | func- |
| Key Vault | kv- |
| Application Insights | appi- |

---

# Deployment Regions

Current deployment

- West Europe
- Germany West Central

Note

Future deployments should use a single Azure region whenever possible to reduce latency and simplify infrastructure management.

---

# Sprint 1 Summary

Azure infrastructure successfully created.

Current Azure Resources

 Resource Group

 Storage Account

 App Service Plan

 Web App

 Azure SQL Server

 Azure SQL Database

Project Status

Infrastructure completed and ready for backend development.