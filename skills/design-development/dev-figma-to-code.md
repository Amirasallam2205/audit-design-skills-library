# dev-figma-to-code

## Description
This skill translates a Figma design into production-ready code. It interprets visual design specifications — including layout, spacing, typography, color, component states, and responsive behavior — and generates the corresponding front-end code. The output respects the project's existing design system, component library, and code conventions. It also highlights any design-to-code mismatches or missing specifications that would prevent accurate implementation.

## Intake
- A Figma link or an exported description of the design frame(s) to be implemented
- Target technology stack (e.g., React + Tailwind CSS, Vue + SCSS, plain HTML/CSS, SwiftUI, Jetpack Compose)
- Relevant design tokens or design system documentation (optional but strongly recommended)
- Existing component library or codebase context (optional — helps avoid duplicate components)
- Responsive breakpoints and behavior expectations (optional — will be inferred from the design if not provided)

## Expected Output
- Production-ready front-end code for the specified design frame(s), including:
  - Component markup (HTML/JSX/TSX/SwiftUI/etc.)
  - Styling (CSS, Tailwind classes, SCSS, styled-components, etc.)
  - Responsive layout handling
  - Component states (default, hover, focus, active, disabled, error, loading, empty)
  - Accessibility attributes (ARIA roles, labels, keyboard interaction patterns)
- A list of design decisions made during code generation (e.g., inferred spacing, color tokens used)
- A list of ambiguities or missing specs that need designer clarification before the code can be finalized
- Inline comments for any non-obvious implementation decisions

## When to Use
Use this skill during the **design-to-development handoff phase** when a Figma design is ready to be implemented. It is especially useful when:
- Bootstrapping a new component from a finalized design
- Generating a first-pass implementation to reduce developer time
- Checking that all design states and variants have a code representation
- Ensuring the implementation stays aligned with the design system
- Speeding up the development of repetitive UI patterns (cards, tables, forms, navigation)
