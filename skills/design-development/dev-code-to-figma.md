# dev-code-to-figma

## Description
This skill reverse-engineers existing front-end code into a structured Figma design specification. It reads component code (HTML, CSS, React, Vue, etc.) and extracts the visual design properties — including layout structure, spacing, typography, color values, border styles, and responsive rules — then documents them in a format that can be recreated in Figma. This is useful for auditing live implementations, creating design documentation for legacy components, or syncing the design library with the current state of the product.

## Intake
- Front-end component code (HTML + CSS, React/TSX, Vue, etc.) — can be pasted directly or provided as a file path reference
- Design system or token mapping file (optional — used to map raw CSS values back to named tokens like `color-primary-500`)
- Figma component naming conventions or folder structure (optional — helps organize the output spec)
- Target Figma version or plugin being used (optional, e.g., Figma Dev Mode, Figma Tokens plugin)

## Expected Output
- A detailed Figma-ready design specification including:
  - **Layout** — frame dimensions, auto-layout direction, alignment, spacing, padding, and gap values
  - **Typography** — font family, weight, size, line height, letter spacing per text element
  - **Colors** — fill, stroke, and background colors mapped to design tokens where possible
  - **Effects** — border radius, shadows, opacity, and blur values
  - **Component variants** — a list of component states and props extracted from the code
  - **Responsive breakpoints** — extracted from media queries or responsive logic
- A mapping of raw CSS/code values to design system tokens (if a token file was provided)
- A list of inconsistencies found between the code and the design system (e.g., hardcoded values that deviate from tokens)
- Suggested Figma component and layer naming based on the code structure

## When to Use
Use this skill when you need to **bring code and design back into alignment**, particularly when:
- A component was built without a corresponding Figma file and needs to be documented
- The live implementation has drifted from the original design and you need to update the Figma source of truth
- Auditing legacy code to create or update the design system library in Figma
- Onboarding a new designer who needs a Figma reference for an existing feature
- Generating design documentation as part of a design debt reduction effort
