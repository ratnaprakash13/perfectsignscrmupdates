# Perfect Signs CRM & Invoicing Integration Work Timeline UI

This is a standalone, single-page responsive timeline application specifically populated with daily work logs through **August 31, 2026** to support client audits, milestone reviews, and invoicing verification.

## Calendar & Milestone Overview (August 2026)
- **Work Days**: All 21 weekdays (Mondays through Fridays) in August 2026 are individually documented.
- **Key Milestones Covered**:
  - **Invoices WebAPI Direct Authentication**: Unified customer registration and login directly with `psinvoiceapi.perfectsignscanada.com` in PostgreSQL (`app_users`).
  - **Multi-Tier Subscription & Quota Enforcement**: Free trial (3 invoices limit), Pro tier ($3 CAD / 200 invoices per month), and Unlimited tier ($5 CAD / month).
  - **Single Sign-On (SSO)**: One-click session handoff between CRM portal (`crm.perfectsignscanada.com`) and Invoices application (`banners.perfectsignscanada.com`).
  - **Multi-Tenancy & Scoping**: Added `user_id` scoping on invoices and clients, paired with an Angular `AuthInterceptor`.
  - **Invoicing Portal Hub in CRM**: Real-time quota progress bar, plan status badges, and 1-click plan upgrade modal.
  - **Production Hosting & Security**: ASP.NET Core 9 WebAPI on IIS, AWS S3 invoice archiving, AWS SES SMTP email dispatch, and IIS ARR reverse proxy.

## Customization & Built-In Admin Tool
1. **Interactive Admin Drawer**: Click the floating gear icon in the bottom-right corner to open the Developer Admin panel.
2. **Real-Time Editing**: Add, update, search, or remove daily logs directly in the browser.
3. **Export**: Click **"Save & Download index.html"** to export the updated state.

## How to Host on IIS / GitHub Pages
1. This repository is pre-configured for GitHub Pages deployment.
2. For IIS, simply copy `index.html` to your IIS webroot and bind to your domain.
