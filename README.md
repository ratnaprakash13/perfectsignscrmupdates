# Perfect Signs Portals, RCM & CRM Work Timeline UI

This is a standalone, single-page responsive timeline application populated with complete daily work logs across **June, July, and August 2026 (73 total daily entries)** to support client audits, milestone reviews, and executive verification.

## Calendar & Milestone Overview (June, July & August 2026)
- **Total Logs**: **73 comprehensive daily entries** (21 entries in June 2026, 22 entries in July 2026, and 30 working day entries in August 2026).
- **Key Milestones Covered**:
  - **August 2026 (30 Working Days)**:
    - **RCM Medical Billing Platform (`https://rcm.perfectsignscanada.com/`)**: Hosted on Windows Server IIS with dedicated SSL/TLS Certificate (HTTPS), medical coding engine (ICD-10/CPT), claims scrubbing, EHR integration, patient co-pay billing, and denial management.
    - **Invoices WebAPI Multi-Tenant Integration**: Unified customer authentication in PostgreSQL (`app_users`), Free (3 lifetime), Pro ($3 CAD / 200 mo), Unlimited ($5 CAD), and Single Sign-On (SSO).
    - **Perfect Signs CRM Visual Builder & SEO**: GrapesJS drag-and-drop editor, CSHTML Razor compiler, AWS SES SMTP dual email alerts, custom quote forms, and Schema.org JSON-LD LocalBusiness SEO.
  - **July 2026 (22 Working Days)**:
    - Cloud infrastructure setup, containerization, AWS S3 document store, GrapesJS custom plugin development, and dynamic client asset streaming.
  - **June 2026 (21 Working Days)**:
    - Initial project scaffolding, ASP.NET Core API foundation, PostgreSQL schema initialization, and basic responsive UI components.

## Customization & Built-In Admin Tool
1. **Interactive Admin Drawer**: Click the floating gear icon in the bottom-right corner to open the Developer Admin panel.
2. **Real-Time Editing**: Add, update, search, or remove daily logs directly in the browser.
3. **Export**: Click **"Save & Download index.html"** to export the updated state.

## How to Host on IIS / GitHub Pages
1. This repository is pre-configured for GitHub Pages deployment.
2. For IIS, simply copy `index.html` to your IIS webroot and bind to your domain.
