# 🌟 UniPro: Zenith Command (v8.0: Multi-Unit Elite)

## 🚀 Overview

**UniPro: Zenith Command** is a highly advanced, single-page application (SPA) designed as a mission control dashboard for tracking university admission exams. Built with a modern, dark, high-contrast Human-Interface-Device (HUD) aesthetic, this system provides real-time countdowns, secure document management (Multi-Admit Card Vault), and personalized note-taking capabilities.

This version, **v8.0**, introduces a major architectural refactor to support **multiple admit cards per university unit**, significantly enhancing its utility for students applying to various faculties within a single institution.

## ✨ Core Features

| Feature | Description | Status |
| :--- | :--- | :--- |
| **Real-Time Chronometer** | Accurate, live countdown timers for all upcoming university exams, displayed in Days, Hours, Minutes, and Seconds. Includes "Critical Status" indicators for exams within 24 hours. | **Fixed & Advanced** |
| **Multi-Admit Card Vault** | **(NEW in v8.0)** Secure local storage and management for multiple PDF admit cards per university, tagged by Unit (e.g., DU A Unit, DU B Unit). | **New/Fixed** |
| **Integrated PDF Viewer** | Reliable, cross-browser inline viewing of uploaded PDF admit cards directly within a modal interface. | **Fixed & Stable** |
| **Dynamic Dashboard** | Displays the top 1-2 most critical upcoming exams in a prominent Hero Section. | **Advanced** |
| **Persistence Layer** | All user data (Pinned Unis, Notes, Admit Cards) is stored locally using `localStorage`. | **Stable** |
| **Filtering & Search** | Ability to filter universities by type (General, Engineering, Medical, etc.) and pin high-priority institutions. | **Stable** |
| **Command Notes** | Dedicated space within each university's detail panel for strategy, seat plan notes, or syllabus reminders. | **Stable** |
| **Advanced UI/UX** | Futuristic, high-contrast dark theme optimized for readability and a dynamic user experience. | **Stable** |

## 🛠️ Technology Stack

This project is a self-contained, client-side application utilizing modern web standards.

* **Frontend Framework:** React 18 (via standalone Babel script)
* **Styling:** Tailwind CSS (via CDN) for rapid, utility-first styling.
* **Language:** JavaScript (ES6+), JSX (handled by Babel).
* **External Assets:** Google Fonts (`Plus Jakarta Sans`, `JetBrains Mono`) and Google Material Symbols (Rounded).

## 📂 Project Structure

This application is designed as a single, highly modular HTML file (`index.html` implicitly), containing all code (HTML, CSS, JavaScript, React components, and data) for maximum portability and ease of distribution.

### Key Internal Components:

* **`useUserData()` Hook:** Manages and persists all user-specific data (pins, notes, admit cards) via `localStorage`. Crucially handles the new `admitCards` array structure.
* **`<LiveTicker>`:** The core component responsible for the accurate, second-by-second countdown logic.
* **`<DeskModal>`:** The detail view for each university, which houses the multi-unit countdowns, the Command Notes, and the primary interface for the Multi-Admit Card Vault.
* **`<PDFViewerModal>`:** Handles the rendering of the Base64 Data URL PDF content in a fullscreen overlay.

## ⚙️ Setup and Installation

Since **Zenith Command** is a self-contained single-page application (SPA) using CDNs, no complex build process is required.

### 1. Local Deployment (Easiest Method)

1.  **Save the Code:** Save the entire provided code block into a file named `index.html`.
2.  **Open:** Double-click `index.html` in your file explorer.
3.  **Run:** The website will open instantly in your default browser.

### 2. Host Deployment (For Web Hosting)

1.  Upload the `index.html` file to your web server (e.g., using Netlify, Vercel, or a traditional host).
2.  The application will run immediately upon access.

> ⚠️ **Note on PDF Storage:** All uploaded admit card files (Base64 data) are stored locally in your browser's `localStorage`. Clearing your browser's cache or using a different browser/device will result in the loss of saved PDF files.

## 🤝 Contribution & Feedback

This project is a demonstration of advanced frontend capabilities focusing on mission-critical utility. Feedback on performance, responsiveness, or new feature requests (e.g., calendar integration, push notifications) is welcome!

***

Developed by **Urfa Hasan Fattah** | Version **v8.0** | 2025# Admission-Exams
