# Pamasahe Catbalogan 🚌

> **Fair Transit Fares & Rate Protection for Catbalogan City, Samar, Philippines**  
> *Dire magpalabi hit pletehan! (Do not overcharge on transit fares!)*

**Pamasahe Catbalogan** is a mobile-first, zero-dependency, offline-ready web application designed to help commuters and drivers in Catbalogan City, Samar calculate accurate fares and verify that passengers are not overcharged.

---

## ✨ Features

- **📱 Mobile-First & Responsive**: Designed for one-hand commuter usage with 44px+ tap targets, high sunlight contrast, and dark/light themes.
- **⚡ 100% Offline Capable**: Zero external dependencies, self-contained single `index.html`, inlined Service Worker, Web App Manifest, and `localStorage` state caching.
- **🧮 Official Fare Matrix Calculation**:
  - Implements official LTFRB fare formulas (effective 28 Sep 2026).
  - Floating-point safe integer centavo arithmetic with quarter-peso (`₱0.25`) rounding.
  - Supports Traditional & Modern Jeepneys, Provincial Buses (Ordinary, Aircon, Deluxe), and UV Express.
  - Dedicated support for local Catbalogan City Hall rates for Tricycles and Habal-Habal.
- **🛡️ "Am I Being Overcharged?" Checker**:
  - Compares driver's requested fare against official rates.
  - Gauge indicator showing Fair, Slightly High, or Overcharge.
  - Generates polite assertion scripts in Waray and English with one-tap copy.
- **🎫 Digital Transit Ticket**:
  - Perforated receipt card showing breakdown, discount savings, and effective date.
  - "Show Driver Fullscreen" mode with large 5.5rem high-contrast display for noisy/night rides.
- **📍 Catbalogan Route Directory**:
  - Pre-seeded popular routes (Pier, Samar College, Maharlika Highway, Bus Terminal, etc.).
  - Custom route builder with `localStorage` persistence.
- **🚨 Scam Prevention & Violation Reporting**:
  - Practical safety tips.
  - Violation reporting form with history, SMS/Email formatting, and City Traffic / LTFRB placeholders.
- **⚙️ Admin & Rate Matrix Manager**:
  - Live editable tariff matrix.
  - JSON import and export.
  - Built-in acceptance test runner (`window.runTests()`).
- **🌐 Bilingual Support**: Instant toggle between English and Waray.
- **🔄 Animated Transit Refresh Screen**: 1.8-second transit splash screen with animated progress and tariff verification stages.

---

## 🚀 Quick Start

1. Clone or download this repository:
   ```bash
   git clone https://github.com/johnmichaelangeloalisna4-hub/pamasahe-catbalogan.git
   ```
2. Open `index.html` in any modern web browser on your phone or desktop:
   - No server, build tools, or npm packages required!
   - Can be added to your mobile home screen as a PWA.

---

## 🧪 Self-Tests

Open Developer Tools in your browser (`F12` or inspect) and run:
```javascript
window.runTests();
```
All 8 LTFRB compliance and Catbalogan edge-case tests will run and log pass/fail status to the console.

---

## 📄 License

MIT License. Open-source for the commuters and community of Catbalogan City.
