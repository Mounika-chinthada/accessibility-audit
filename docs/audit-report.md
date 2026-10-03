# Accessibility Audit Report

## Website Audited

- Website: india.gov.in
- Audit Tool: Google Chrome Lighthouse
- Accessibility Score: 89

  

## Automated Accessibility Findings

### WEB-001 — ARIA

**Finding:** [role]s are not contained by their required parent element.

**Evidence:** Lighthouse reported that some ARIA child roles are not contained by their required parent elements.

**User Impact:** Screen-reader users may have difficulty interpreting the affected interface structure.

**Recommended Fix:** Review the affected ARIA roles and ensure they are placed within their required parent elements, or use appropriate semantic HTML.


### WEB-002 — Color Contrast

**Finding:** Background and foreground colors do not have a sufficient contrast ratio.

**Evidence:** Lighthouse reported insufficient foreground/background color contrast.

**User Impact:** Users with low vision may have difficulty reading the affected content.

**Recommended Fix:** Adjust the foreground and background colors to provide sufficient contrast.


### WEB-003 — List Structure

**Finding:** List items (<li>) are not contained within <ul>, <ol> or <menu> parent elements.

**Evidence:** Lighthouse reported that some <li> elements are not contained within the required list parent elements.

**User Impact:** Screen-reader users may receive incorrect information about list structure.

**Recommended Fix:** Place <li> elements inside the appropriate <ul>, <ol>, or <menu> parent element.


### WEB-004 — Image Alt Attribute

**Finding:** Image elements do not have [alt] attributes that are redundant text.

**Evidence:** Lighthouse reported an image alt-attribute issue.

**User Impact:** Assistive-technology users may have difficulty understanding the affected images.

**Recommended Fix:** Provide appropriate, non-redundant alt text for applicable images and appropriate empty alt text for decorative images.

## Repository Architecture Finding

### ARCH-001 — Client and Server Boundaries Not Yet Implemented

**Finding:** The repository contains separate `client/` and `server/` directories, but the directories currently contain only placeholder files and do not yet contain application implementation.

**Evidence:** The repository structure includes dedicated `client/` and `server/` directories, while the initial project skeleton does not yet contain frontend or backend implementation.

**User/Project Impact:** Without initial implementation boundaries, it is not yet possible to verify the separation between frontend responsibilities and backend responsibilities.

**Remediation Priority:** Medium

**Recommended Fix:** Establish the client/server boundaries with a minimal setup-ready implementation, keeping UI code inside `client/`, API and server-side logic inside `server/`, shared documentation inside `docs/`, and automated tests inside `tests/`.


## Manual Accessibility Checks

Lighthouse also reported 10 additional items to manually check.

These are separate from the four automated findings documented above. The individual details of those 10 manual checks were not captured in the available audit evidence, so they are not listed individually in this report.


## Conclusion

The audited website received an Accessibility score of 89 in Lighthouse.

Four automated accessibility findings were documented for the audited website. Lighthouse also identified 10 additional items requiring manual accessibility checks.

In addition, one repository architecture finding was documented for the project skeleton: the `client/` and `server/` boundaries are defined, but their initial application implementations are not yet present.
