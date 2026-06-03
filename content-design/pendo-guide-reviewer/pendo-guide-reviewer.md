---
name: pendo-guide-reviewer
description: Review and critique Pendo guides designed in Figma against TR standards. Use this skill whenever someone shares Pendo guide content, copy, or a description of a guide they're designing and wants feedback, a review, or wants to know if it meets standards. Trigger on phrases like "review my Pendo guide", "does this guide follow standards", "check my guide copy", "is this the right template", "what should my button say", "is this guide ready to publish", "review this walkthrough", or any time someone pastes or describes Pendo guide content (title, body, buttons, anchors). Also trigger when someone asks which guide type or template to use for a specific use case.
---

# Pendo Guide Reviewer

A skill for reviewing TR Pendo guides against the four governing standards: the TR Pendo Guides Library (visual/structural specs), the Ready-to-Review templates (approved content patterns), Saffron content principles, and the TR word list.

## What this skill reviews

When a user shares a Pendo guide (copy, description, or screenshot), evaluate it across four dimensions:

1. **Template selection** — Is the right guide type being used for the use case?
2. **Content standards** — Does the copy follow Saffron voice, tone, and grammar rules?
3. **Word list compliance** — Are banned words avoided? Are preferred TR terms used?
4. **Visual/structural specs** — Are layout, component, and behavior specs followed?

---

## Step 0: Orient to the CoE process stage

Ask (or infer from context) where the guide is in the TR 4-step CoE process:

| Stage | What to focus on |
|---|---|
| **Step 1 — Define strategy** | Is the guide initiative, target audience, triggers, and segmentation defined? |
| **Step 2 — Collaborate & build** | Is an approved template being used? Does it align with the Guides Library? |
| **Step 3 — Test guide** | Run a full review pass (content, copy, structure, word list). Guide status should be Draft. |
| **Step 4 — Approve & publish** | Final sign-off. Confirm all standards met before manual or scheduled publish. |

If the stage isn't clear, ask: *"Is this guide in draft for feedback, or are you preparing it for approval and publish?"*

See `references/coe-process.md` and `assets/Pendo_CoE_Best_Practices.webp` for the full process.

---

## Step 1: Identify the guide type

Determine which guide type the user is working on. Ask if not clear.

| Guide type | Icon | Use case |
|---|---|---|
| **Feature announcement** | Bell | Single-screen notification for a new/updated feature |
| **Major announcement** | Megaphone/bullhorn | Significant product moment — release, event, community |
| **Step-through tutorial** | Circle-info | Multi-step walkthrough anchored to UI elements |
| **Contextual guide / tooltip** | Circle-info (popover) | Triggered by interaction; clarifies a specific UI element |
| **Feedback survey** | Message-dots | Collecting satisfaction ratings + optional open text |
| **Warning** | Triangle-exclamation | Planned outage or service degradation |
| **Completion** | Circle-check | Final step of a walkthrough |

Once identified, load the matching section from `references/guide-type-rules.md` for detailed specs.

---

## Step 2: Run the content review checklist

Apply ALL of the following checks regardless of guide type. Flag every issue clearly.

### Voice and tone
- [ ] Does tone match the guide type? (Feature = Confident; Tutorial = Confident + Precise; Contextual = Precise only; Announcement = Passionate + Confident; Feedback = Genuine)
- [ ] No marketing language ("industry-leading", "easier than ever", "best-in-class")
- [ ] No platitudes or filler phrases
- [ ] Active voice used (passive is acceptable only when shifting blame from the user)

### Title
- [ ] Sentence case (first word + proper nouns only)
- [ ] No period at end
- [ ] No exclamation point (exception: major announcements only, and only if warranted)
- [ ] Does NOT start with "New:" as a prefix (for feature announcements)
- [ ] Correct word count for type: Feature/Announcement = 4–6 words; Tutorial step = 3–5 words; Contextual = 1–4 words

### Body copy
- [ ] Correct sentence count for type: Feature/Announcement = 2–4 sentences; Tutorial step = 1–3 sentences (max 1 paragraph); Contextual = 1–2 sentences
- [ ] First sentence adds new information — does NOT restate the title
- [ ] User-goal focused, not UI-centric
- [ ] Concise — no padding, no filler
- [ ] Specific — no vague claims like "a better way to manage your documents"
- [ ] Does not explain domain concepts the audience already knows
- [ ] Does not attempt to document every option visible on screen

### Button labels
- [ ] Primary CTA is a specific, descriptive verb — NOT "Got it", "OK", "Close" (unless contextually correct — see type rules)
- [ ] Tutorial buttons use standard: Back, Next, Done (no Back on first step)
- [ ] Secondary button is present only when appropriate
- [ ] No "Learn more" as standalone link text — must be descriptive

### Anchor text / links
- [ ] Descriptive, not generic ("Read the diagnostics guide" not "Learn more")
- [ ] Only present when the resource adds real value

### Word list compliance (see `references/word-list-rules.md`)
- [ ] No banned words: invalid, fatal, forbidden, fail/failure
- [ ] "Please" and "sorry" used only when system is at fault
- [ ] "Click" replaced with "select"
- [ ] "Log in / log out" replaced with "sign in / sign out"
- [ ] "Submit" replaced with goal-specific verb
- [ ] No inclusive language violations (blacklist/whitelist/master/slave)

### Grammar and punctuation
- [ ] You/your used to address user directly
- [ ] We/our used for system or company references
- [ ] Periods at end of complete sentences; none on headings, buttons, or standalone links
- [ ] Oxford comma used in lists of 3+
- [ ] Ampersand (&) spelled out as "and" unless part of proper name
- [ ] No ALL CAPS except acronyms, file extensions, trademarked names

---

## Step 3: Check structural/visual specs

Cross-reference against the library specs (see `references/visual-specs.md`).

Key checks:
- Dialog width: 548 px (standard), 232 px (tooltip/popover)
- Text alignment: left
- Overlay background: #000000 at 30% (for modal dialogs)
- Embedded guides: flexible width, placed at top of page
- Correct icon for guide type (see guide type table above)
- Image sizes respected: min 500×200 px, max 500×500 px (or 548×240 px for announcement 1.2)
- Close (X) button present on all guide types
- Step counter format: "Step N of N" (tutorial only)
- Popover text limit: up to 40 words + optional title

---

## Step 4: Deliver the review

Structure your review as follows:

**Guide type identified:** [name]
**Template match:** ✅ Correct / ⚠️ Check / ❌ Wrong — [brief reason]

Then for each issue found:

> **[Area: Title / Body / Button / Link / Word list / Structure]**
> ❌ Issue: [what's wrong, quoted from the guide]
> ✅ Suggestion: [specific fix]
> 📖 Rule: [which standard this comes from]

End with a summary:
- **Ready to publish:** Yes / No / Needs minor revision
- **Priority fixes:** [numbered list of the most important changes]
- **Quick wins:** [any easy improvements even if not blockers]

---

## Reference files

Load these when you need detail beyond what's in this file:

- `references/guide-type-rules.md` — Per-type content rules (when to use, voice, title/body/button requirements)
- `references/visual-specs.md` — Layout dimensions, image sizes, icon mapping, behavior specs
- `references/word-list-rules.md` — Approved terms, banned words, TR-specific vocabulary
- `references/content-principles.md` — Full Saffron 5 Cs, grammar, punctuation, capitalization rules
- `references/coe-process.md` — TR Pendo CoE 4-step guide creation process (Define strategy → Collaborate & build → Test guide → Approve & publish)
- `assets/Pendo_CoE_Best_Practices.webp` — Visual diagram of the CoE 4-step process

---

## Common mistakes to watch for (from the library)

These patterns appear in the legacy Figma library (TR_Pendo_Guides_Library.pdf) but do NOT follow the Ready-to-Review content standards. Flag these if seen:

- "Got it!" on non-completion steps — only appropriate on final confirmation step
- "NEW:" prefix in titles — not allowed per content guidelines
- Vague body copy like "This layout is designed to announce planned outage..." — placeholder text must be replaced with specific content
- "Anchor text" as actual link text — must be replaced with descriptive label
- "Label text" as secondary button text — must be replaced with specific action
- "We are pleased to announce..." — marketing language; not allowed
- "Built from the ground up to provide you with the best that technology can provide" — platitude; not allowed
- "Learn more" alone as anchor text — must be descriptive
