# Library Management Configurations

## Student Information
- **Student Name:** Shavindi R. Aloka
- **Student Number:** [ඔබේ ශිෂ්‍ය අංකය මෙහි ඇතුළත් කරන්න]
- **Slack Handle:** [ඔබේ Slack නම]
- **GCP Project ID:** [ඔබේ Google Cloud Project ID එක]

---

## Project Description
This repository serves as the centralized configuration server repository for the Library Management microservice architecture. It manages and externalizes configuration properties (such as database connections, Eureka service registry settings, and cloud storage properties) for all microservices using Spring Cloud Config Server.

---

## Technology Stack
- **Configuration Management:** Spring Cloud Config Server
- **Version Control:** Git / GitHub
- **Environment Properties:** YAML (`application.yaml`)

---

## Repository Structure
- `platform/` - Configurations related to platform components (API Gateway, Eureka, etc.)
- `services/` - Configurations specific to individual microservices (MySQL and MongoDB-backed services)
- `application.yaml` - Global configuration properties

---

## Setup / Getting Started Instructions
1. Ensure the Config Server is pointed to this repository URL in its `application.yaml` or `bootstrap.yaml`:
   ```yaml
   spring:
     cloud:
       config:
         server:
           git:
             uri: [https://github.com/Shavindi0609/Library-Management-Configurations](https://github.com/Shavindi0609/Library-Management-Configurations)
