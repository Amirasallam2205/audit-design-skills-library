# vqa-design-comparison

## Description
This skill performs a visual quality assurance (VQA) review by comparing a live or staged implementation against the original Figma design. It identifies visual discrepancies across layout, spacing, typography, color, component states, and responsive behavior. The output is a structured audit report that helps designers and developers quickly identify and fix deviations before a feature ships to production.

## Intake
- A Figma design link or exported design screenshots for the feature/component under review
- A screenshot, screen recording, or URL of the live/staged implementation to compare against
- The target viewport(s) or device(s) to review (e.g., desktop 1440px, tablet 768px, mobile 375px)
- A list of specific states or interactions to check (optional — e.g., hover, focus, error state, empty state)
- Design system or brand guidelines document (optional — used to validate token usage)

## Expected Output
- A structured VQA audit report organized by severity:
  - 🔴 **Critical** — deviations that break functionality, brand identity, or accessibility (must fix before launch)
  - 🟡 **Major** — visible deviations from the design that affect quality (should fix before launch)
  - 🟢 **Minor** — small inconsistencies that are acceptable but worth noting (fix if time permits)
- For each issue found:
  - Description of the discrepancy
  - Expected value (from design)
  - Actual value (from implementation)
  - Suggested fix or action item
  - Screenshots or annotated references (if provided as input)
- A summary scorecard showing total issues by severity and affected component areas
- A "pass/fail" recommendation for the feature

## When to Use
Use this skill during the **visual quality assurance phase**, after a feature has been implemented and before it is approved for production release. It is especially useful when:
- Conducting a formal design QA review as part of the release process
- A designer wants to quickly audit an implementation without manually comparing every pixel
- Checking that responsive breakpoints match the design across multiple device sizes
- Validating that all component states (hover, focus, disabled, error, empty) were implemented correctly
- Performing a design system compliance check to ensure tokens and styles are used consistently
