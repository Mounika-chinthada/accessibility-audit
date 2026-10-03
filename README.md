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
├── server/
├── docs/
│   └── audit-report.md
├── screenshots/
├── tests/
└── README.md
