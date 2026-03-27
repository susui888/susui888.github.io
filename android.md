---
layout: default
title: Library Management System — Android App
permalink: /android/
---

<div class="card border-0 shadow-sm mb-5" style="background-color: #fdfdfb; border: 1px solid #eee5d8 !important;">
    <div class="card-body p-4">
        <div class="d-flex align-items-start mb-3"> <div class="bg-custom-brown-light p-2 rounded-3 me-3" style="background-color: rgba(139, 69, 19, 0.1);">
                <i class="bi bi-android2 fs-3" style="color: #8B4513;"></i>
            </div>
            <div class="flex-grow-1">
                <div class="d-flex justify-content-between align-items-center">
                    <h3 class="mb-0 text-custom-brown" style="font-family: 'Geist Sans', sans-serif;">CoolLib — Native Android Client</h3>

                    <a href="https://github.com/susui888/CoolLib_Android/actions/workflows/android-ci.yml" class="d-print-none">
                        <img src="https://github.com/susui888/CoolLib_Android/actions/workflows/android-ci.yml/badge.svg" alt="Android CI/CD">
                    </a>
                </div>

                <div class="mt-1 d-flex flex-wrap gap-1">
                    <span class="badge rounded-pill" style="background-color: #3DDC84; color: #000;">Jetpack Compose</span>
                    <span class="badge rounded-pill" style="background-color: #8B4513;">Kotlin</span>
                    <span class="badge rounded-pill" style="background-color: #6c757d;">MVVM</span>
                    <span class="badge rounded-pill bg-dark">Hilt DI</span>
                </div>
            </div>
        </div>

        <p class="text-muted mb-4">
            A high-performance library management mobile application featuring a <b>"Book-Style"</b> custom design system. 
            Built with <b>Clean Architecture</b>, it provides an offline-first experience with real-time synchronization to the Spring backend.
        </p>

        <div class="d-flex gap-2">
            <a href="https://github.com/susui888/CoolLib_Android" target="_blank" class="btn btn-sm btn-outline-dark rounded-pill px-3">
                <i class="bi bi-github me-1"></i> Source Code
            </a>
            <a href="#core-features" class="btn btn-sm btn-outline-brown rounded-pill px-3" style="border-color: #8B4513; color: #8B4513;">
                <i class="bi bi-palette me-1"></i> Design System
            </a>
        </div>
    </div>
</div>

## <i class="bi bi-layers-half me-2"></i> Architectural Philosophy

**CoolLib Android** is engineered using **Modern Android Development (MAD)** practices. By implementing a reactive data pipeline and strict layer separation, the app ensures a fluid user experience even under complex data states and varying network conditions.

## <i class="bi bi-cpu-fill me-2"></i> Key Technical Wins

* **Clean Architecture**: Implemented strict **MVVM** with isolated Data, Domain, and UI layers using **Kotlin-First** principles for maximum maintainability.
* **Performance Tuning**: Reduced data load times by **60%** via **Coroutines (`async/awaitAll`)** for concurrent repository-level data mapping and transformation.
* **Dependency Injection**: Engineered a robust DI graph with **Hilt**, utilizing custom **Qualifiers** (`@IoDispatcher`) for granular threading control.
* **Reactive Pipeline**: Built a real-time data flow using **StateFlow/SharedFlow** integrated with **Room** for a reliable "Offline-First" experience.
* **Quality Assurance**: Maintained system stability with **MockK** unit tests and **Compose Rule** UI tests covering core business logic.

---

### <i class="bi bi-diagram-3-fill me-2"></i> Data Flow Architecture
{% include graph-android-dataflow.html %}

### <i class="bi bi-check-all me-2"></i> Single Source of Truth (SSOT)
{% include graph-android-ssot.html %}

---

## <i class="bi bi-stack me-2"></i> Tech Stack

* **UI Framework**: Jetpack Compose, Material 3, Coil (Image Loading), Compose Navigation
* **Logic & Concurrency**: MVVM, Use Cases, Coroutines, Kotlin Flow, Hilt (DI)
* **Data Persistence**: Retrofit (REST API), Moshi (JSON), Room (Local DB), DataStore

## <i class="bi bi-command me-2" id="core-features"></i> Core Features

* **Loan Tracking**: Optimized list views for "Active" vs. "History" using status-driven UI components.
* **Smart Insights**: Real-time calculation of library metrics such as "Due Soon" and "Overdue" status.
* **Intelligent Search**: Multi-criteria filtering logic with localized caching for instantaneous results.
* **Book-Style UI**: A custom-themed design system with a signature paper-like palette and textured components.

## <i class="bi bi-phone-vibrate me-2"></i> UI Preview

{% include gif.html
id="androidDemo"
path="/assets/img/android1.gif"
title="CoolLib Android App Preview"
icon="bi-android2"
description="Demonstrating: Book Search, Real-time Validation, and Borrowing Flow." %}

<hr class="my-5">

<div class="small text-muted text-center">
    <p><i class="bi bi-code-slash me-1"></i> Engineered by Ryan Su &copy; 2026</p>
</div>