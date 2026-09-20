# System Architecture Specification: E2FY Sovereign Platform

## 1. Executive Overview
The **E2FY (Enrich Experience For Yog) Sovereign Platform** is a high-performance, single-file static web application designed to host Sanatana Dharma frameworks, neuroscience, thermodynamics, and the Life-Algo book series for Gen-Z and Gen-Alpha audiences.

## 2. Technology Stack & Core Principles
* **Architecture:** Single-Page Application (SPA) built entirely within a unified self-contained file (`index.html`) to guarantee zero build-step complexity and instant execution.
* **Styling Engine:** Tailwind CSS via CDN with custom Tailwind configuration extending dark mode (`class`), custom brand colors (`brand-*`, `accent-*`), and typography fonts.
* **Iconography:** FontAwesome 6.5.1 (`font-awesome`).
* **Typography:** Google Fonts (`Inter`, `Outfit`, `Noto Sans Tamil`, `Mukta Malar`).
* **Backend Integration:** FormSubmit AJAX API (`https://formsubmit.co/ajax/e2fyusers@gmail.com`) for zero-config email notification dispatch on static hosting.

## 3. Component & View Routing Architecture
The platform manages view transitions dynamically via client-side DOM manipulation without page reloads:
* `#view-home`: Platform overview, master formula, and interactive Principle Carousel (0 to 5).
* `#view-life`: E2FY-Life Book Series Hub.
* `#view-life-part1`: Detailed landing page for *Life-Algo Series Part I - The Master Code*, featuring multi-language book edition tabs (English, Tamil, Hindi) and trailer video series.
* `#view-edu`: E2FY-Edu (Coming Soon with early access email capture).
* `#view-health`: E2FY-Health (Coming Soon with early access email capture).

## 4. Modal Sub-Systems
* **Video Modal (`#video-modal`):** Responsive modal overlay embedding privacy-enhanced YouTube (`youtube-nocookie.com`) players with direct fallback links to eliminate Error 153.
* **Audit Modal (`#audit-modal`):** Interactive diagnostic wizard evaluating 16 core queries and generating a real-time Sovereignty Score.