# vqa-accessibility-audit

## Description
This skill performs a focused accessibility audit on a design or implementation to verify compliance with WCAG (Web Content Accessibility Guidelines) standards. It evaluates the design against criteria including color contrast ratios, keyboard navigation, focus management, screen reader support, touch target sizes, and semantic structure. The output is an actionable accessibility report that helps the team identify and remediate accessibility issues before launch.

## Intake
- A Figma design link, exported screenshots, or a URL to the live/staged implementation
- The target WCAG conformance level (A, AA, or AAA — defaults to WCAG 2.1 AA if not specified)
- A description of the interactive elements in the design (e.g., buttons, form fields, modals, dropdowns) — optional but improves analysis
- Any known assistive technologies to test against (e.g., VoiceOver, NVDA, JAWS) — optional
- User personas that include users with disabilities (optional — used to contextualize findings)

## Expected Output
- An accessibility audit report organized by WCAG success criteria, including:
  - **1.1 Text Alternatives** — missing or inadequate alt text for images and icons
  - **1.3 Adaptable** — reliance on sensory characteristics (color alone, shape, position)
  - **1.4 Distinguishable** — color contrast ratios for all text and interactive elements
  - **2.1 Keyboard Accessible** — components that are not operable via keyboard
  - **2.4 Navigable** — missing focus indicators, skip navigation, or logical focus order
  - **3.3 Input Assistance** — form labels, error messages, and validation feedback
  - **4.1 Compatible** — semantic HTML structure and ARIA usage issues
- For each issue:
  - WCAG success criterion violated (e.g., 1.4.3 Contrast Minimum)
  - Severity (Critical, Major, Minor)
  - Description of the issue
  - Specific element or location in the design
  - Recommended fix
- A summary of pass/fail status per WCAG criterion
- An overall accessibility score and conformance level assessment

## When to Use
Use this skill during the **visual QA phase** whenever accessibility compliance is required, which should be for every feature and component. It is especially critical when:
- Preparing a feature for production release where accessibility compliance is mandated
- Reviewing a new design component for inclusion in the design system
- Conducting an accessibility remediation effort on an existing feature
- Validating that a redesign maintains or improves accessibility compared to the previous version
- Performing an audit ahead of a formal accessibility certification or legal compliance review
