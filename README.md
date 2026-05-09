# 📋 PO Request Portal

A lightweight web application that replaces email-based Purchase Order requests with a structured, trackable system. Built for internal use at M-KOPA Kenya by the Demand & Supply Planning team.

---

## 🔍 The Problem

Before this tool, all PO requests were handled over Outlook email:

- Colleagues attached PFIs and typed loose descriptions into emails
- No standard format — missing fields, unclear quantities, vague delivery dates
- Amendments arrived as replies in the same thread, causing version confusion
- No central log, no request IDs, no audit trail
- Easy to miss requests under high inbox volume

---

## ✅ The Solution

A two-screen web portal that gives every PO request a unique ID, a structured form, and a full audit trail — and gives the planner a live dashboard to manage, update, and track all requests in one place.

---

## 🖥 Features

### Request Form (for colleagues)
- Structured input — supplier, item, quantity, unit, delivery date, department
- PFI file upload at point of request
- Urgency flag
- Amendment support — link to original Request ID
- Auto-generates a unique Request ID on submission
- Confirmation flow on submit

### Planner Dashboard (for the demand planner)
- Summary stats — total requests, pending, raised, amended
- Sortable table — sorted by delivery date ascending, pending first
- Search by requester, supplier, item, or request ID
- Filter by status — Pending / Raised / Amended / Cancelled
- Click-to-open side panel with full request details
- Update PO number and status directly from the panel

---

## 🗂 Project Structure

```
po-request-portal/
│
├── po-request-portal.html   # Single-file app — all HTML, CSS, JS included
└── README.md
```

This is a **frontend-only prototype**. All data is held in memory during the session. A backend version with persistent storage is planned for Phase 2.

---

## 🚀 Getting Started

### Option 1 — Open locally
Download `po-request-portal.html` and open it in any modern browser. No installation, no dependencies, no server needed.

### Option 2 — Host on GitHub Pages
1. Fork or clone this repo
2. Go to **Settings → Pages**
3. Set source to `main` branch, root folder
4. GitHub will publish a live URL you can share with your team

---

## 📸 Screenshots

| Request Form | Planner Dashboard |
|---|---|
| Structured form with all required fields, PFI upload, and urgency flag | Live table with search, filter, stats, and a side panel for updates |

---

## 🛣 Roadmap

This prototype is Phase 2 of a two-phase automation plan.

| Phase | Description | Status |
|-------|-------------|--------|
| Phase 1 | Microsoft Forms + Power Automate — no-code, live at M-KOPA | 🟡 In progress |
| Phase 2a | This prototype — frontend-only, single HTML file | ✅ Complete |
| Phase 2b | Full-stack version — React frontend + Node.js/Express API | 🔲 Planned |
| Phase 2c | Database integration — Supabase (Postgres + file storage) | 🔲 Planned |
| Phase 2d | Email notifications — auto-confirm to requester on PO raised | 🔲 Planned |
| Phase 2e | Authentication — login per user, role-based access | 🔲 Planned |

---

## 🧱 Planned Tech Stack (Phase 2b+)

| Layer | Technology |
|-------|------------|
| Frontend | React |
| Backend | Node.js + Express |
| Database | Supabase (PostgreSQL) |
| File storage | Supabase Storage (PFI uploads) |
| Email | Nodemailer |
| Hosting | Vercel (frontend) + Railway (backend) |

---

## 👤 Author

**Brian Karugu**  
Demand & Planning Officer — M-KOPA Kenya  
BSc Purchasing & Supplies Management, Dedan Kimathi University  
Software Engineering Student — Zindua School (2026 cohort)

---

## 📄 License

This project is for internal use and portfolio purposes. Not licensed for commercial distribution.