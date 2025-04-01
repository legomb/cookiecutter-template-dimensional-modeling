# PROPOSAL: {{cookiecutter.project_name}}

## Overview

The process is simple: first we define the problem, and based on that we propose one or more possible solutions.

## Problem Statement

What problem do we want to solve?

### Requirements

#### Functional Requirements

- FR001:
- FR002:

#### Technical Requirements

- TR001:
- TR002:

#### Out of Scope

- OOS001:
- OOS002:

### Business Process

Identify the business process.

```mermaid
sequenceDiagram
	actor ActorA
	participant Salesforce

	ActorA ->> Salesforce: Create Account
```

## Proposed Solution

### Entities

#### Entity-Relationship Diagram (ERD)

```mermaid
erDiagram
    CUSTOMER ||--o{ ORDER : places
    CUSTOMER {
        string name
        string custNumber
        string sector
    }
    ORDER ||--|{ LINE-ITEM : contains
    ORDER {
        int orderNumber
        string deliveryAddress
    }
    LINE-ITEM {
        string productCode
        int quantity
        float pricePerUnit
    }
```

#### Facts

#### Dimensions

### Deliverables

Number | Name | Description | Effort
---------|----------|---------|---------
 1 | Approval | Business user approves this proposal | Med
 2 | B2 | C2 | Low
 3 | B3 | C3 | High

### Roadmap

```mermaid
gantt
    title Project Roadmap
    dateFormat YYYY-MM-DD
    section Section
        A task          :a1, 2014-01-01, 30d
        Another task    :after a1, 20d
    section Another
        Task in Another :2014-01-12, 12d
        another task    :24d
```
