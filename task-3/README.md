# Task 3 — Semantic HTML5 & Accessible Component Architecture

## Objective

Build a structural foundation for an enterprise dashboard using semantic HTML5, accessible form controls, WCAG 2.1 principles, and a structured DOM hierarchy.

## Pages

The Task 3 implementation includes:

- `index.html` — Main enterprise dashboard
- `dashboard.html` — Dashboard overview
- `users.html` — User management page
- `components/README.md` — Accessible component documentation

## Semantic HTML5 Structure

The pages use semantic HTML5 elements including:

- `<header>`
- `<nav>`
- `<main>`
- `<section>`
- `<article>`
- `<aside>`
- `<footer>`

## Accessibility Features

The implementation includes:

- Proper heading hierarchy
- Descriptive navigation labels
- Keyboard-accessible links and buttons
- Table captions and column scopes
- Explicit `<label>` elements for form controls
- `<fieldset>` and `<legend>` for grouped form controls
- Required form validation attributes
- Appropriate input types and autocomplete attributes
- Accessible dialog structure using `<dialog>`
- `aria-current`, `aria-labelledby`, `aria-controls`, and `aria-haspopup` where appropriate

## Validation

All three HTML pages were validated using the W3C HTML Validator.

| Page | Validation Result |
|---|---|
| `index.html` | 0 errors, 0 warnings |
| `dashboard.html` | 0 errors, 0 warnings |
| `users.html` | 0 errors, 0 warnings |

## Repository Structure

```text
task-3/
├── index.html
├── dashboard.html
├── users.html
└── components/
    └── README.md
