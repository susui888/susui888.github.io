---
layout: default
title: Android Project
permalink: /android/
---
# 🤖 CoolLib - Android App

<div style="margin: 10px 0 30px 15px;"> <a href="https://github.com/susui888/CoolLib_Android" target="_blank" 
       style="text-decoration: none; 
              display: inline-flex; 
              align-items-center; 
              border: 1.5px solid #8B4513; 
              color: #8B4513; 
              background-color: transparent; 
              padding: 6px 16px; 
              border-radius: 20px; 
              font-weight: 600; 
              font-size: 14px; 
              transition: all 0.3s ease;">
        <svg style="margin-right: 8px;" width="18" height="18" fill="currentColor" viewBox="0 0 16 16">
            <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"/>
        </svg>
        View Source Code
    </a>
</div>

**CoolLib** is a high-performance library management ecosystem built with **Jetpack Compose** and **Clean Architecture**. It features a "Book-Style" custom design system and enterprise-grade data handling.

## 🚀 Key Technical Wins

- **Clean Architecture**: Implemented strict **MVVM** with isolated layers (Data, Domain, UI) using **Kotlin First** principles for high maintainability.
- **Performance Tuning**: Reduced data load times by **60%** via **Coroutines (`async/awaitAll`)** for concurrent repository-level data mapping.
- **Dependency Injection**: Engineered a robust DI graph with **Hilt**, utilizing custom **Qualifiers** (`@IoDispatcher`) for granular threading control.
- **Reactive Pipeline**: Built a real-time data flow using **StateFlow/SharedFlow** integrated with **Room** for an "Offline-First" experience.
- **Quality Assurance**: Maintained system stability with **MockK** unit tests and **Compose Rule** UI tests covering core business logic.

{% include graph-android-dataflow.html %}

{% include graph-android-ssot.html %}

## 🛠 Tech Stack

- **UI**: Jetpack Compose, Material 3, Coil (Image Loading), Compose Navigation.
- **Logic**: MVVM, Use Cases, Coroutines, Flow, Hilt (DI).
- **Data**: Retrofit (REST API), Moshi (JSON), Room (Local DB), SharedPreferences.

## ✨ Core Features

- **Loan Tracking**: Optimized list views for "Active" vs. "History" using status-driven UI components.
- **Smart Insights**: Real-time calculation of library metrics such as "Due Soon" and "Overdue" items.
- **Intelligent Search**: Multi-criteria filtering logic with localized caching for instantaneous results.
- **Book-Style UI**: Custom-themed design system with a signature paper-like palette and textured components.

{% include gif.html
id="androidDemo"
path="/assets/img/android1.gif"
title="CoolLib Android App Preview"
icon="bi-android2"
description="Demonstrating: Book Search, Real-time Validation, and Borrowing Flow." %}