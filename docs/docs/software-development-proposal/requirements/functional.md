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

## Introduction

[//]: <> (Provide an overview of the functional requirements and their importance in the software development process.)

## User Roles and Permissions

[//]: <> (Define the different user roles and their respective permissions within the software, such as administrators, managers, and end-users.)

The application must implement the following set of roles:

- Administrator
- User

Each user can have one of the following roles for each module:

- Module Coordinator
- Teaching Assistant

Below is a table describing actions each user and role is allowed to take.

|                                 | Administrator | Module Coordinator | Teaching Assistant |
|:-------------------------------:|:-------------:|:------------------:|:------------------:|
| View modules                    | Yes           | Yes                | Yes                |
| Create modules                  | Yes           | -                  | -                  |
| Update modules                  | Yes           | Yes                | -                  |
| Delete modules                  | Yes           | -                  | -                  |
| View labs                       | Yes           | Yes                | Yes                |
| Create labs                     | Yes           | Yes                | -                  |
| Update labs                     | Yes           | Yes                | -                  |
| Delete labs                     | Yes           | Yes                | -                  |
| View lab schedules              | Yes           | Yes                | Yes                |
| Create lab schedules            | Yes           | Yes                | -                  |
| Update lab schedules            | Yes           | Yes                | -                  |
| Delete lab schedules            | Yes           | Yes                | -                  |
| View users                      | Yes           | -                  | -                  |
| Create users                    | Yes           | -                  | -                  |
| Update users                    | Yes           | -                  | -                  |
| Delete users                    | Yes           | -                  | -                  |
| View users allocated to modules | Yes           | Yes                | -                  |
| Add users to modules            | Yes           | -                  | -                  |
| Remove users from modules       | Yes           | -                  | -                  |
| View users allocated to labs    | Yes           | Yes                | -                  |
| Add users to labs               | Yes           | Yes                | -                  |
| Remove users from labs          | Yes           | Yes                | -                  |
| Send questionnaires to users    | Yes           | -                  | -                  |
| Fill-in questionnaires          | Yes[^1]       | Yes                | Yes                |
| Approve pre-allocation requests | Yes           | Yes                | -                  |
| Deny pre-allocation requests    | Yes           | Yes                | -                  |
| Run allocation algorithms       | Yes           | -                  | -                  |
| Delete all data in the system   | Yes           | -                  | -                  |

[^1]: Also allowed to fill-in questionnaires on behalf of other users.

## Core Features and Functionality

[//]: <> (Describe the main features and functionality of the software, including any essential components that are critical to its operation.)

### API Endpoints

[//]: <> (Detail the API endpoints requirements, including the HTTP methods, the request and response formats, and the expected response codes.)

### Data Management

[//]: <> (Explain how the software will handle data storage, retrieval, and manipulation, including any database requirements.)

### Integration with External Systems

[//]: <> (Describe any necessary integration with external systems, such as third-party APIs or other software components.)

### Reporting and Analytics

[//]: <> (Outline the reporting and analytics capabilities of the software, including any custom reports or dashboards that need to be developed.)

## Security and Compliance

[//]: <> (Discuss the security and compliance requirements for the software, including data protection, user authentication, and any industry-specific regulations that must be adhered to.)

The application must integrate with Azure Active Directory and support Single Sign-on.

## Performance and Scalability

[//]: <> (Describe the performance and scalability requirements for the software, including any expected load and response times, as well as the ability to handle future growth.)

## Accessibility and Usability

[//]: <> (Outline the accessibility and usability requirements for the software, ensuring that it meets the needs of all users, including those with disabilities.)

## Localization and Internationalization

[//]: <> (Discuss any localization and internationalization requirements, such as support for multiple languages and cultural considerations.)

## Testing and Quality Assurance

[//]: <> (Explain the testing and quality assurance processes that will be used to ensure the software meets the functional requirements and is free of defects.)

## Documentation and Training

[//]: <> (Describe the documentation and training materials that will be provided to help users understand and effectively use the software.)

## Summary

[//]: <> (Summarize the functional requirements and emphasize their importance in the successful development and implementation of the software.)
