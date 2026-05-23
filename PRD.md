# KASHLET — PRODUCT REQUIREMENTS DOCUMENT (PRD)

## 1. Product Overview

Kashlet is a modern billing and financial workspace designed for freelancers, creators, and small businesses to create invoices, track payments, and generate receipts within a fast, intuitive interface.

The product focuses on speed, clarity, and trust — allowing users to manage financial records without complexity or accounting knowledge.

---

## 2. Problem Statement

Freelancers and small businesses face challenges such as:
- slow and complex invoice creation tools
- difficulty tracking payment statuses
- manual conversion of invoices into receipts
- scattered client and financial records
- tools that are either too advanced or too basic

There is a gap between:
simple templates and enterprise accounting systems

Kashlet fills this gap with a lightweight, structured billing system.

---

## 3. Product Goals

- Enable users to create invoices in under 2 minutes
- Provide clear payment tracking (pending, paid, overdue)
- Automatically convert invoices into receipts
- Maintain organized client and business records
- Offer a clean dashboard for financial visibility
- Ensure fast, mobile-friendly usability

---

## 4. Target Users

- Freelancers (designers, developers, writers)
- Small business owners
- Vendors and service providers
- Creators managing paid work
- Startup teams needing lightweight billing

---

## 5. Core Features (MVP Scope)

### Authentication
- Sign up / sign in
- Basic session management

### Dashboard
- Total invoices overview
- Paid vs unpaid summary
- Recent invoices list
- Quick create invoice action

### Invoice System
- Create invoice (guided form)
- Add client details
- Add items/services
- Quantity + pricing calculation
- Tax/discount support (basic)
- Notes section
- Invoice number generation

### Invoice Management
- Status tracking (Draft / Pending / Paid)
- Invoice editing
- Invoice deletion
- Search and filtering

### Receipt System
- Convert paid invoice → receipt
- Receipt generation automatically

### Export & Sharing
- PDF export
- Download invoice/receipt
- Shareable link (optional MVP enhancement)

### Client Management
- Save reusable clients
- Edit client details

---

## 6. User Flow (Core System)

1. User signs in
2. Lands on dashboard
3. Creates invoice
4. Adds client + items
5. Preview invoice
6. Downloads or shares invoice
7. Marks invoice as paid
8. Invoice converts to receipt
9. Data stored in dashboard history

---

## 7. System Architecture

### Frontend Structure
- Dashboard layout system
- Component-based UI (invoice, table, forms)
- Reusable UI components (buttons, inputs, modals)

### Data Model

#### User
- id
- name
- email
- business name

#### Client
- id
- userId
- name
- email
- phone
- address

#### Invoice
- id
- userId
- clientId
- items[]
- totalAmount
- status (draft/pending/paid)
- createdAt
- dueDate

#### Receipt
- id
- invoiceId
- issuedAt

---

## 8. UX Principles

- Reduce friction in invoice creation
- Keep dashboard information scannable
- Prioritize clarity over decoration
- Maintain consistent hierarchy
- Use real-time feedback for actions

---

## 9. Design Direction (High-Level)

- Clean SaaS dashboard style
- Minimal but modern UI
- Soft borders, no heavy shadows
- Strong typography hierarchy
- Calm neutral color system with accent color for actions

---

## 10. Technical Direction (For Vibe Coding Tools)

- Web application (responsive)
- Component-based architecture
- CRUD-based data system
- Local storage or Firebase/Supabase backend
- PDF generation support
- Real-time UI updates

---

## 11. Success Metrics

- Invoice creation completed in under 2 minutes
- Users can easily distinguish invoice statuses
- Smooth navigation between dashboard and invoice system
- No confusion in workflow steps
- Clean export (PDF accuracy + readability)

---

## 12. Exclusions (MVP Boundaries)

- No full accounting system
- No payroll or tax automation
- No bank integrations
- No enterprise ERP features

Focus is strictly on:
FAST + SIMPLE billing workflow.

---

## 13. Product Positioning

Kashlet is not an accounting system.

It is:
A lightweight billing workspace for fast invoice and receipt generation.
