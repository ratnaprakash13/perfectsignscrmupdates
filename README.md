# Perfect Signs Portals, RCM & CRM Work Timeline UI

This is a standalone, single-page responsive timeline application populated with daily work logs across **30 working days in August 2026** to support client audits, milestone reviews, and executive verification.

## Calendar & Milestone Overview (August 2026 - 30 Working Days)
- **Work Days**: 30 comprehensive daily entries from **August 01, 2026 through August 30, 2026** covering every phase of development, deployment, and security hardening.
- **Key Milestones Covered**:
  - **RCM Medical Billing Platform (`https://rcm.perfectsignscanada.com/`)**:
    - Complete Revenue Cycle Management (RCM) web portal for healthcare practices, clinics, and surgical centers.
    - Medical coding engine (ICD-10-CM, CPT, HCPCS Level II) with automated claims scrubber (NCCI edits).
    - EHR/EMR interface integration, ANSI 837 claims generation, and 835 ERA remittance parsing.
    - Patient statement generator, online co-pay payment portal, and denial management with A/R recovery aging tracking.
    - HIPAA & PIPEDA compliance architecture with role-based access control (RBAC).
    - **Production Hosting on Windows Server IIS**: Dedicated application pool, web.config SPA rewrite rules, and **SSL/TLS Certificate (HTTPS)** binding.
  - **Invoices WebAPI Direct Authentication & Multi-Tenancy**:
    - Unified customer registration and login directly with `psinvoiceapi.perfectsignscanada.com` in PostgreSQL (`app_users`).
    - Multi-tenant data scoping (`user_id` foreign keys) on invoices and clients with Angular `AuthInterceptor`.
  - **Multi-Tier Subscription & Quota Enforcement**:
    - Free trial (3 lifetime invoices limit), Pro tier ($3 CAD / 200 monthly invoices), and Unlimited tier ($5 CAD / month).
    - Single Sign-On (SSO) one-click session handoff between CRM (`crm.perfectsignscanada.com`) and Invoices (`banners.perfectsignscanada.com`).
    - Invoicing Portal Hub card in CRM dashboard with live quota progress bar and in-app upgrade modal.
  - **Perfect Signs CRM Core & AWS Cloud Architecture**:
    - GrapesJS drag-and-drop visual layout editor with live view and styling locks.
    - Server-side Razor CSHTML compilation and 1-click publishing to IIS webroot.
    - AWS SES SMTP dual email alert dispatch (`email-smtp.ca-central-1.amazonaws.com:587`) for quote requests and ticketing notifications.
    - Parallel AWS API Gateway serverless WebAPI dispatch (`ContactUsEmail`).
    - Comprehensive SEO optimization (titles, descriptions, OpenGraph/Twitter cards, Alberta geo-tags, Schema.org JSON-LD LocalBusiness).

## Customization & Built-In Admin Tool
1. **Interactive Admin Drawer**: Click the floating gear icon in the bottom-right corner to open the Developer Admin panel.
2. **Real-Time Editing**: Add, update, search, or remove daily logs directly in the browser.
3. **Export**: Click **"Save & Download index.html"** to export the updated state.

## How to Host on IIS / GitHub Pages
1. This repository is pre-configured for GitHub Pages deployment.
2. For IIS, simply copy `index.html` to your IIS webroot and bind to your domain.
