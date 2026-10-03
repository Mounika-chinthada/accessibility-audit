# Accessibility Baseline & Repository Architecture Audit

## Project Overview

This project documents an accessibility baseline audit and repository architecture setup for the website [india.gov.in](https://india.gov.in/).

The accessibility audit was performed using Google Chrome Lighthouse.

## Accessibility Audit

- **Website Audited:** india.gov.in
- **Audit Tool:** Google Chrome Lighthouse
- **Accessibility Score:** 89

### Automated Findings

The Lighthouse audit identified the following accessibility findings:

1. **ARIA**
   - `[role]s are not contained by their required parent element`

2. **Color Contrast**
   - `Background and foreground colors do not have a sufficient contrast ratio.`

3. **List Structure**
   - `List items (<li>) are not contained within <ul>, <ol> or <menu> parent elements.`

4. **Image Alt Attribute**
   - `Image elements do not have [alt] attributes that are redundant text.`

Lighthouse also reported **10 additional items to manually check**.

## Repository Structure

```text
accessibility-audit/
├── client/
│   └── .gitkeep
├── server/
│   └── .gitkeep
├── docs/
│   ├── audit-report.md
│   └── accessibility-audit-final.csv
├── screenshots/
├── tests/
│   └── .gitkeep
└── README.md
```
## Architecture Boundaries

This project uses a monorepo-style structure with separate areas for frontend, backend, documentation, screenshots, and tests.

- `client/` — Reserved for frontend application and user interface code.
- `server/` — Reserved for backend API and server-side application logic.
- `docs/` — Contains the accessibility audit report and audit CSV.
- `screenshots/` — Contains screenshots captured as evidence during the Lighthouse audit.
- `tests/` — Reserved for automated tests.
- `README.md` — Provides project architecture, setup, and implementation guidance.

The client and server directories establish a clear separation between frontend and backend responsibilities. Documentation and testing remain separate from application code.

## Local Setup

### Prerequisites

- Git
- Node.js
- npm

### Clone the Repository

```bash
git clone https://github.com/Mounika-chinthada/accessibility-audit.git
cd accessibility-audit
```

### Project Setup

The repository currently provides the initial project skeleton. The `client/`, `server/`, and `tests/` directories are prepared for implementation.

Frontend dependencies will be installed from the `client/` directory when the client application is initialized.

Backend dependencies will be installed from the `server/` directory when the server application is initialized.

The current repository can be reviewed without installing application dependencies because the initial skeleton contains documentation, audit evidence, and placeholder files.

## First Vertical Feature Slice

The first planned vertical feature slice is an accessible audit-results view.

The feature will connect the frontend, backend, and test layers:

```text
User
  ↓
Client
  ↓
Server API
  ↓
Audit Data
  ↓
Client Audit Results View
```

The `client/` layer will provide the user interface for viewing accessibility findings.

The `server/` layer will provide the API and server-side logic required to serve audit data.

The `tests/` layer will contain tests for the feature.


The feature will be implemented with accessibility in mind, including keyboard navigation, visible focus states, semantic HTML, and appropriate accessible names.












