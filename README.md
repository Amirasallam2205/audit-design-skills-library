# audit-design-skills-library
Shared library of Claude Skills for the Audit Design team.

This library contains AI skills that help the Audit Design team accelerate their end-to-end design process — from gathering requirements all the way through to visual quality assurance. Each skill is a focused prompt that Claude can use to complete a specific task, with documented intake, expected outputs, and guidance on when to use it.

---

## Skill Naming Convention

Every skill follows a **prefix naming convention** that indicates which phase of the design process it belongs to:

| Prefix | Phase |
|--------|-------|
| `req-` | Requirements |
| `dev-` | Design & Development |
| `vqa-` | Visual Quality Assurance |

---

## Skills Index

### 📋 Requirements (`req-`)

Skills for gathering, analyzing, and formalizing design requirements.

| Skill | Description |
|-------|-------------|
| [`req-analyze-requirements`](skills/requirements/req-analyze-requirements.md) | Transforms raw, unstructured input into organized, prioritized design requirements |
| [`req-write-user-stories`](skills/requirements/req-write-user-stories.md) | Converts requirements into well-formed user stories with acceptance criteria |
| [`req-acceptance-criteria`](skills/requirements/req-acceptance-criteria.md) | Generates detailed, testable acceptance criteria for a design deliverable or feature |

### 🎨 Design & Development (`dev-`)

Skills for translating between Figma designs and code, in both directions.

| Skill | Description |
|-------|-------------|
| [`dev-figma-to-code`](skills/design-development/dev-figma-to-code.md) | Translates a Figma design into production-ready front-end code |
| [`dev-code-to-figma`](skills/design-development/dev-code-to-figma.md) | Reverse-engineers existing code into a structured Figma design specification |

### 🔍 Visual Quality Assurance (`vqa-`)

Skills for reviewing and validating design implementations.

| Skill | Description |
|-------|-------------|
| [`vqa-design-comparison`](skills/visual-qa/vqa-design-comparison.md) | Compares a live implementation against the original Figma design and reports discrepancies |
| [`vqa-accessibility-audit`](skills/visual-qa/vqa-accessibility-audit.md) | Audits a design or implementation for WCAG accessibility compliance |

---

## Recommended Workflow

These skills are designed to work together in sequence across the design lifecycle:

```
req-analyze-requirements
        ↓
req-write-user-stories
        ↓
req-acceptance-criteria
        ↓
  dev-figma-to-code
  dev-code-to-figma
        ↓
vqa-design-comparison
vqa-accessibility-audit
```

---

## Contributing

When adding a new skill to this library:
1. Place the skill file in the appropriate phase folder under `skills/`
2. Name the file using the correct phase prefix (e.g., `req-`, `dev-`, `vqa-`)
3. Use the standard skill template structure: **Description**, **Intake**, **Expected Output**, **When to Use**
4. Add the skill to the index table in this README
