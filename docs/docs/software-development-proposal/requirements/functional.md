---
title: Functional Requirements
layout: default
nav_order: 1
parent: Requirements
grand_parent: Software Development Proposal
---

[//]: <> (These requirements define the functions and functionality within and from the software system.)
[//]: <> (Examples of functional requirements include authentication, authorization levels, compliance to laws or regulations, and external interfaces.)

# Functional Requirements
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Hosting

Lorem ipsum...

## Security and Identity

Lorem ipsum...

### Authentication

The application must integrate with Azure Active Directory and support Single Sign-on.

### Authorization

The application must implement the following set of roles:

- Administrator
- User

User can have one of the following roles for each module:

- Module Coordinator
- Lab Coordinator
- Teaching Assistant

Below is a table describing actions each role is allowed to take.

|                                 | Administrator | Module Coordinator | Lab Coordinator | Teaching Assistant |
|:-------------------------------:|:-------------:|:------------------:|:---------------:|:------------------:|
| View modules                    | Yes           | Yes                | Yes             | Yes                |
| Create modules                  | Yes           | -                  | -               | -                  |
| Update modules                  | Yes           | Yes                | Yes             | -                  |
| Delete modules                  | Yes           | -                  | -               | -                  |
| View labs                       | Yes           | Yes                | Yes             | Yes                |
| Create labs                     | Yes           | Yes                | Yes             | -                  |
| Update labs                     | Yes           | Yes                | Yes             | -                  |
| Delete labs                     | Yes           | Yes                | Yes             | -                  |
| View lab schedules              | Yes           | Yes                | Yes             | Yes                |
| Create lab schedules            | Yes           | Yes                | Yes             | -                  |
| Update lab schedules            | Yes           | Yes                | Yes             | -                  |
| Delete lab schedules            | Yes           | Yes                | Yes             | -                  |
| View users                      | Yes           | -                  | -               | -                  |
| Create users                    | Yes           | -                  | -               | -                  |
| Update users                    | Yes           | -                  | -               | -                  |
| Delete users                    | Yes           | -                  | -               | -                  |
| View users allocated to modules | Yes           | Yes                | Yes             | -                  |
| Add users to modules            | Yes           | -                  | -               | -                  |
| Remove users from modules       | Yes           | -                  | -               | -                  |
| View users allocated to labs    | Yes           | Yes                | Yes             | -                  |
| Add users to labs               | Yes           | Yes                | Yes             | -                  |
| Remove users from labs          | Yes           | Yes                | Yes             | -                  |
| Send questionnaires to users    | Yes           | -                  | -               | -                  |
| Fill-in questionnaires          | Yes           | Yes[^1]            | Yes[^1]         | Yes[^1]            |
| Approve pre-allocation requests | Yes           | Yes                | Yes             | -                  |
| Deny pre-allocation requests    | Yes           | Yes                | Yes             | -                  |
| Run allocation algorithms       | Yes           | -                  | -               | -                  |
| Delete all data in the system   | Yes           | -                  | -               | -                  |

[^1]: Only on the user's own behalf.

### Data Protection

- Encryption at rest
- Data integrity (Row versioning)
- Concurrency
