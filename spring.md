---
layout: default
title: Library Management System — Spring Backend
permalink: /spring/
---

<div class="card border-0 shadow-sm mb-5" style="background-color: #fdfdfb; border: 1px solid #eee5d8 !important;">
    <div class="card-body p-4">
        <div class="d-flex align-items-center mb-3">
            <div class="bg-custom-brown-light p-2 rounded-3 me-3" style="background-color: rgba(139, 69, 19, 0.1);">
                <i class="bi bi-database-fill fs-3" style="color: #8B4513;"></i>
            </div>
            <div>
                <h3 class="mb-0 text-custom-brown" style="font-family: 'Geist Sans', sans-serif;">CoolLib — Distributed Library Core API</h3>
                <div class="mt-1 d-flex flex-wrap gap-1">
                    <span class="badge rounded-pill" style="background-color: #8B4513;">Spring Boot 3.4</span>
                    <span class="badge rounded-pill" style="background-color: #6c757d;">PostgreSQL</span>
                    <span class="badge rounded-pill" style="background-color: #0d6efd;">JWT Security</span>
                    <span class="badge rounded-pill bg-dark">Kotlin</span>
                </div>
            </div>
        </div>

        <p class="text-muted mb-4">
            A high-performance backend ecosystem engineered with <b>Clean Architecture</b>. 
            It implements a strict separation between <b>JPA Entities</b> and <b>DTOs</b>, 
            serving as the central orchestration hub for both Android (Kotlin) and iOS (SwiftUI) clients.
        </p>

        <div class="d-flex gap-2">
            <a href="https://github.com/susui888/demo2" target="_blank" class="btn btn-sm btn-outline-dark rounded-pill px-3">
                <i class="bi bi-github me-1"></i> Source Code
            </a>
            <a href="#core-features" class="btn btn-sm btn-outline-brown rounded-pill px-3" style="border-color: #8B4513; color: #8B4513;">
                <i class="bi bi-shield-lock me-1"></i> API Security
            </a>
        </div>
    </div>
</div>

## <i class="bi bi-layers-half me-2"></i> Project Overview

**CoolLib Backend** is a robust RESTful service built with **Spring Boot 3.4** and **Kotlin**. Beyond standard CRUD operations, it manages complex business logic layers to ensure data consistency, security, and seamless synchronization across the mobile ecosystem.

## <i class="bi bi-diagram-3-fill me-2"></i> Key Technical Wins

* **Layered Architecture**: Strictly follows the **Controller-Service-Repository** pattern, ensuring complete decoupling between business logic and data access layers.
* **Secure Sessions**: Integrated **Spring Security** with **JWT (JSON Web Tokens)** to provide a stateless authentication mechanism tailored for mobile clients.
* **Persistence Layer**: Leverages **PostgreSQL** and **Spring Data JPA**, ensuring the atomicity of borrowing operations through **@Transactional** services.
* **Performance Optimization**: Reduced network overhead via **DTO Projections** and optimized database indexing for high-speed book searches.

---

### <i class="bi bi-cpu-fill me-2"></i> System Architecture
{% include graph-architecture.html %}

### <i class="bi bi-lock-fill me-2"></i> Authentication Flow
{% include graph-authentication.html %}

---

## <i class="bi bi-server me-2"></i> Tech Stack

* **Core Framework**: Spring Boot 3.4, Kotlin (JVM 17), Maven
* **Security**: JWT, Spring Security, BCrypt Password Hashing
* **Data Management**: PostgreSQL, Spring Data JPA, Hibernate ORM
* **Standards**: RESTful API Design, Docker-Ready Deployment

## <i class="bi bi-shield-check me-2" id="core-features"></i> Core Features

* **Identity Management**: Secure user registration and token-based login systems.
* **Advanced Search**: Server-side pagination, multi-parameter filtering, and full-text search capabilities.
* **Transaction Logic**: Atomic borrowing/returning operations with real-time inventory validation and user quota enforcement.
* **Standardized Responses**: Unified JSON response structures with custom error codes to ensure cross-platform compatibility.

## <i class="bi bi-cloud-arrow-up-fill me-2"></i> Mobile Connectivity

Both **Android (Jetpack Compose)** and **iOS (SwiftUI)** clients interact with this backend through standard REST endpoints. All protected resources require an `Authorization: Bearer <token>` header, maintaining data integrity and user privacy across the CoolLib ecosystem.

<hr class="my-5">

<div class="small text-muted text-center">
    <p><i class="bi bi-code-slash me-1"></i> Developed with passion by Ryan Su &copy; 2026</p>
</div>