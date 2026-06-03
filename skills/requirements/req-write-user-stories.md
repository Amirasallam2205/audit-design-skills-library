# req-write-user-stories

## Description
This skill converts design requirements or feature descriptions into well-formed user stories following the standard "As a [user], I want [goal], so that [benefit]" format. It also generates acceptance criteria for each story using the Given-When-Then (GWT) format and suggests relevant edge cases the team should design for. The output helps bridge the gap between stakeholder needs and the design/development team's understanding of what needs to be built.

## Intake
- A set of design requirements or a feature description (can be in any format: bullet points, paragraphs, a Figma link description, or plain notes)
- Target user persona(s) or a brief description of the end user (optional but recommended)
- Project context and goals (optional)

## Expected Output
- A set of user stories written in the standard format: *"As a [user type], I want to [action/goal], so that [benefit/reason]"*
- For each user story:
  - Acceptance criteria written in Given-When-Then (GWT) format
  - Suggested edge cases to design for
  - Story size estimate hint (small / medium / large) based on complexity
- A brief summary of what is covered and what may need further elaboration

## When to Use
Use this skill **after requirements have been analyzed and organized** (ideally after running `req-analyze-requirements`) and before starting design work or development tickets. It is especially useful when:
- Translating a product brief or stakeholder request into sprint-ready tickets
- Ensuring the design team and development team share a common understanding of the feature
- Preparing for sprint planning or backlog grooming sessions
- Creating the definition of done criteria for a design before it goes to visual QA
