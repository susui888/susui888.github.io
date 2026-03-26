---
layout: default
title: Library Management System — iOS App
permalink: /ios/
---

<div class="card border-0 shadow-sm mb-5" style="background-color: #fdfdfb; border: 1px solid #eee5d8 !important;">
    <div class="card-body p-4">
        <div class="d-flex align-items-center mb-3">
            <div class="bg-custom-brown-light p-2 rounded-3 me-3" style="background-color: rgba(139, 69, 19, 0.1);">
                <i class="bi bi-apple fs-3" style="color: #8B4513;"></i>
            </div>
            <div>
                <h3 class="mb-0 text-custom-brown" style="font-family: 'Geist Sans', sans-serif;">CoolLib — Native iOS Client</h3>
                <div class="mt-1 d-flex flex-wrap gap-1">
                    <span class="badge rounded-pill bg-dark">SwiftUI</span>
                    <span class="badge rounded-pill" style="background-color: #F05138;">Swift 6</span>
                    <span class="badge rounded-pill" style="background-color: #8B4513;">SwiftData</span>
                    <span class="badge rounded-pill" style="background-color: #6c757d;">MVVM</span>
                </div>
            </div>
        </div>

        <p class="text-muted mb-4">
            A premium, high-performance library management experience leveraging modern Apple frameworks. 
            Built with <b>Clean Architecture</b> and <b>Structured Concurrency</b>, it delivers an offline-first workflow synced with the Spring backend.
        </p>

        <div class="d-flex gap-2">
            <a href="https://github.com/susui888/CoolLib2_iOS" target="_blank" class="btn btn-sm btn-outline-dark rounded-pill px-3">
                <i class="bi bi-github me-1"></i> Source Code
            </a>
            <a href="#core-features" class="btn btn-sm btn-outline-brown rounded-pill px-3" style="border-color: #8B4513; color: #8B4513;">
                <i class="bi bi-command me-1"></i> Features
            </a>
        </div>
    </div>
</div>

## <i class="bi bi-layers-half me-2"></i> Architectural Philosophy

**CoolLib iOS** is a testament to **Protocol-Oriented Programming (POP)**. By utilizing the latest **Swift 6** features and a declarative UI approach, the application achieves a highly testable and decoupled codebase that prioritizes both developer velocity and end-user fluidity.

## <i class="bi bi-cpu-fill me-2"></i> Key Technical Wins

* **Protocol-Oriented Architecture**: Implemented **Clean Architecture (MVVM)** with strict abstraction layers, utilizing **Swift Protocols** for decoupled and mockable business logic.
* **Modern Concurrency**: Leveraged **Structured Concurrency (Async/Await)** to handle parallel data fetching and repository mapping, eliminating callback-based complexity.
* **Declarative Persistence**: Integrated **SwiftData** for model-centric local storage, enabling seamless "Offline-First" synchronization and state management.
* **Reactive UI Pipeline**: Engineered a responsive binding layer using the **Observation** framework and **Combine**, ensuring real-time UI consistency across complex views.
* **Quality Assurance**: Built a comprehensive test suite using **XCTest**, focusing on repository mapping accuracy and domain entity integrity.

---

### <i class="bi bi-diagram-3-fill me-2"></i> iOS Data Flow
{% include graph-ios-dataflow.html %}

### <i class="bi bi-check-all me-2"></i> Single Source of Truth
{% include graph-ios-ssot.html %}

---

## <i class="bi bi-stack me-2"></i> Tech Stack

* **UI Framework**: SwiftUI, SF Symbols, Custom ViewModifiers, Core Animation
* **Logic & Concurrency**: MVVM, Use Cases, Async/Await, Observation, Combine
* **Data Management**: URLSession (REST API), SwiftData (Persistence), Codable

## <i class="bi bi-app-indicator me-2" id="core-features"></i> Core Features

* **Loan Management**: Sophisticated list tracking for "Active" vs. "History" with real-time status indicators.
* **Library Analytics**: Dynamic computation of "Due Soon" and "Overdue" metrics directly from the local data store.
* **Advanced Search**: Multi-parameter filtering engine optimized for smooth performance with large book catalogs.
* **Signature Design**: A custom-crafted SwiftUI theme featuring a parchment-inspired palette and paper-textured UI components.

<hr class="my-5">

<div class="small text-muted text-center">
    <p><i class="bi bi-code-slash me-1"></i> Engineered by Ryan Su &copy; 2026</p>
</div>