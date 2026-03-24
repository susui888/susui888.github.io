---
layout: default
title: Spring Project
permalink: /spring/
---
# CoolLib - Library Management API

**CoolLib Backend** is a stateless REST service built with **Spring Boot 3.4** and **Kotlin**, serving as the central hub for the CoolLib mobile ecosystem (Android/iOS).

## 🚀 Key Technical Wins

- **Architecture**: **Stateless REST** design with a strict layered approach (Web, Service, Data).
- **Security**: **JWT-based Auth** via Spring Security for secure mobile session management.
- **Data**: **PostgreSQL** + **Spring Data JPA** for reliable persistence and performance.
- **Scalability**: Pure API-driven service optimized for native mobile clients.

## 🛠 Tech Stack

- **Server**: Spring Boot 3.4, Kotlin (JVM 17), Maven.
- **Security**: JWT, Spring Security, BCrypt.
- **Database**: PostgreSQL, Spring Data JPA.

## 📊 Core Features

- **Auth**: JWT-secured login & registration.
- **Catalog**: Advanced book search & filtering.
- **Transactions**: Borrowing process & loan history.
- **Categories**: Genre-based navigation.

## 📱 Mobile Connectivity

Android and iOS clients connect via JSON. Secure endpoints require the `Authorization: Bearer <token>` header.

