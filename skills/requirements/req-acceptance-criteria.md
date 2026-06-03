# req-acceptance-criteria

## Description
This skill generates detailed acceptance criteria for a design deliverable or feature. It defines precise, testable conditions that must be satisfied for the design to be considered complete and correct. The criteria cover functional behavior, visual fidelity, responsiveness, accessibility standards, and edge/error states. The output serves as a shared checklist between designers, developers, and QA reviewers to ensure the delivered design meets all expectations.

## Intake
- A user story or feature description (can be provided as text, a link to a Jira/Linear ticket, or a Figma frame description)
- Design mockups or wireframes (optional — a Figma link or screenshot description works)
- Any relevant design system or brand guidelines (optional)
- Accessibility requirements or target WCAG level (optional, defaults to WCAG 2.1 AA)

## Expected Output
- A numbered list of acceptance criteria organized into the following sections:
  1. **Functional Criteria** — what the component/feature must do
  2. **Visual/UI Criteria** — pixel, spacing, color, and typography requirements
  3. **Responsive & Adaptive Criteria** — expected behavior across breakpoints or device types
  4. **Accessibility Criteria** — keyboard navigation, screen reader support, contrast ratios, ARIA labels, etc.
  5. **Edge & Error States** — empty states, loading states, error messages, character limits, etc.
- A summary of open questions or assumptions made while generating the criteria

## When to Use
Use this skill **after user stories have been written** (ideally after running `req-write-user-stories`) and before a design is handed off to development or sent to visual QA. It is especially useful when:
- Creating a formal design handoff document
- Defining the exit criteria for a design ticket
- Setting up test cases for visual QA review
- Ensuring accessibility requirements are captured before development begins
- Reducing ambiguity and back-and-forth during the development phase
