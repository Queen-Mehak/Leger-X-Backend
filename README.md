# ✦ LedgerX

> A modern financial intelligence platform designed to bring personal finance, planning, simulation, risk awareness, and intelligent guidance into one connected experience.

---

## 🌌 About LedgerX

**LedgerX** is a financial-management and financial-intelligence web application.

The goal is simple:

> **Turn scattered financial information into a clear, interactive view of the user's financial life.**

Instead of treating budgeting, goals, investments, loans, risk, simulations, reports, and financial guidance as separate tools, LedgerX brings them together into one connected platform.

The current project is built using **React + Vite**, with **React Router**, reusable React components, and an existing HTML/JavaScript layer that is being progressively integrated into the new architecture.

---

## ✨ Key Features

### 🏠 Authentication & Onboarding

- User registration
- Login flow
- Onboarding
- Forgot-password flow
- Authentication-aware navigation

### 📊 Financial Dashboard

- Financial overview
- Quick statistics
- Recent activity
- Financial timeline
- Navigation across major financial modules

### 💰 Finance Management

- Income tracking
- Expense tracking
- Monthly cash-flow calculations
- Financial profile
- Spending categories
- Budget-oriented planning

### 🎯 Financial Goals

- Create financial goals
- Track goal progress
- Plan contributions
- Monitor target dates

### 📈 Investments

- Investment records
- Portfolio-oriented views
- Investment allocation
- Performance-oriented calculations

### 💳 Loans & Debt

- Loan information
- Outstanding balance
- Repayment tracking
- Debt summaries

### 🔮 Digital Twin & Simulation

LedgerX is designed to go beyond simple record keeping.

Users can explore financial assumptions and possible future outcomes through:

- Digital Twin concepts
- Simulation Lab
- Future projections
- Goal scenarios

### ⚠️ Risk Centre

A dedicated area for:

- Financial risk assessment
- Risk indicators
- Risk-oriented recommendations

### 🤖 AI Advisor

LedgerX includes an AI-advisor direction intended to provide contextual financial guidance based on permitted user information.

> AI-generated information should be treated as guidance and not as guaranteed financial advice.

### 📑 Reports & Timeline

- Financial reports
- Timeline views
- Aggregated financial information
- Future export/report capabilities

### ⚙️ Administration

A dedicated administrative area is planned for:

- User management
- Moderation
- Platform-level controls

---

## 🧩 Architecture

```text
                    ┌─────────────────────┐
                    │      LedgerX UI     │
                    │     React + Vite    │
                    └──────────┬──────────┘
                               │
                    ┌──────────▼──────────┐
                    │    React Router     │
                    │  Application Routes │
                    └──────────┬──────────┘
                               │
          ┌────────────────────┼────────────────────┐
          │                    │                    │
          ▼                    ▼                    ▼
   Shared Components     Page Components      Legacy Bridge
   ─────────────────     ───────────────      ─────────────
   Navbar                Dashboard            LegacyPage
   Sidebar               Finances                  ↓
   AdminSidebar          Goals              Existing HTML
   Button                Investments         + JavaScript
   StatCard              Loans
                         Risk
                         Advisor
                         Reports
                               │
                               ▼
                    ┌─────────────────────┐
                    │    Backend Layer    │
                    │ Node.js + Express   │
                    │      Planned        │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │       MySQL         │
                    │   Planned Database  │
                    └─────────────────────┘
