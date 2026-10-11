# حافظي (Hafizi) — نظام إدارة بيانات العملاء والفواتير

<p align="right" dir="rtl">
منصة خفيفة ومستقلة تعمل بالكامل داخل المتصفح لإدخال بيانات العملاء، وإدارة الفواتير والخدمات، وحفظها محلياً، وتوليد إيصالات وفواتير بصيغة PDF ثنائية اللغة (عربي / إنجليزي).
</p>

---

## Overview / نظرة عامة

**حافظي (Hafizi)** is an open-source, serverless customer record manager and PDF receipt generator created specifically for Arabic-speaking freelancers, independent consultants, and small business owners.

The application operates **100% client-side** in the user's browser, eliminating the need for database servers, backend APIs, or monthly hosting subscriptions. Client records are persisted using browser `localStorage`, and receipts can be rendered and downloaded as PDF files instantly.

---

## Key Features / المميزات الرئيسية

- **واجهة مستخدم عربية سلسة (RTL Support):** Designed natively with RTL directionality and Arabic typography (`Noto Naskh Arabic`).
- **إدارة بيانات العملاء والخدمات:** Record brand name, customer name, contact details, address, service category, project notes, price, and currency.
- **دعم متعدد للعملات:** Built-in support for Arab and international currencies (SAR, AED, IQD, MAD, DZD, KWD, EGP, USD, EUR) with localized symbols and labels.
- **توليد فواتير وإيصالات PDF (Bilingual Receipts):** Dynamically generates formatted, print-ready bilingual (Arabic/English) invoices using `html2canvas` and `jsPDF`.
- **حفظ محلي فوري (Local Persistence):** Automatically saves customer entries directly in the browser's `localStorage` without external cloud dependencies.
- **سجل المعاملات:** Inspect and manage past customer records, download receipts repeatedly, or remove deleted transactions.
- **صفر تكاليف تشغيل (Zero Server Infrastructure):** Consists of a single static web document requiring no Node.js build process, database, or backend server.

---

## Technology Stack / التقنيات المستخدمة

- **Markup & Layout:** HTML5 semantic structure.
- **Styling:** Vanilla CSS3 (Custom properties, Responsive Flexbox & Grid layouts, CSS keyframe animations).
- **Typography:** Google Fonts (`Noto Naskh Arabic`).
- **Programming Language:** Vanilla JavaScript (ES6+).
- **Libraries (CDN):**
  - [html2canvas (v1.4.1)](https://html2canvas.hertzen.com/) — DOM-to-canvas rendering.
  - [jsPDF (v2.5.1)](https://parall.ax/products/jspdf) — Client-side PDF document generation.
- **Storage:** Browser `localStorage` API.

---

## Architecture & How It Works
