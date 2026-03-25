---
layout: default
title: iOS Project
permalink: /ios/
---
# 🍎 CoolLib - iOS App

<div style="margin: 10px 0 30px 15px;"> <a href="https://github.com/susui888/CoolLib2_iOS" target="_blank" 
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

**CoolLib** is a high-performance library management ecosystem built with **SwiftUI** and **Clean Architecture**. It delivers a premium native experience leveraging modern iOS frameworks and reactive design patterns.

## 🚀 Key Technical Wins

- **Protocol-Oriented Architecture**: Implemented **Clean Architecture (MVVM)** with strict abstraction layers, utilizing **Swift Protocols** for decoupled and testable logic.
- **Modern Concurrency**: Leveraged **Structured Concurrency (Async/Await)** to handle parallel data fetching and repository mapping without callback nesting.
- **Declarative Persistence**: Integrated **SwiftData** for efficient, model-centric local storage and seamless "Offline-First" state synchronization.
- **Reactive UI Pipeline**: Engineered a responsive data binding layer using **Observation** and **Combine**, ensuring fluid UI updates across complex view hierarchies.
- **Quality Assurance**: Built a comprehensive test suite using **XCTest**, focusing on repository mapping accuracy and core domain entity validation.

{% include graph-ios-dataflow.html %}

{% include graph-ios-ssot.html%}

## 🛠 Tech Stack

- **UI**: SwiftUI, SF Symbols, Custom ViewModifiers, Animation frameworks.
- **Logic**: MVVM, Use Cases, Async/Await (Concurrency), Combine.
- **Data**: URLSession (REST API), SwiftData (Persistence), Codable (JSON).

## ✨ Core Features

- **📖 Loan Management**: Sophisticated list tracking for "Active" vs. "History" with real-time status indicators.
- **📈 Library Analytics**: Dynamic computation of "Due Soon" and "Overdue" metrics directly from the local store.
- **🔍 Advanced Search**: Multi-parameter filtering engine with optimized performance for large book catalogs.
- **🎨 Signature Design**: Custom-crafted SwiftUI theme with a parchment palette and paper-texture UI components.