# Guide Type Rules Reference

Detailed content rules per guide type. Load this file when reviewing a specific guide type.

---

## Feature Announcement (Bell icon)

**When to use:** A single-screen notification introducing a new or updated feature to existing users. Triggered by a release or first encounter with the feature area. Not for major releases or events — use Major Announcement instead.

**Voice and tone:** Confident. State what's new without buildup or hype. Passionate: tell the user why it matters to them. Be enthusiastic, not excited.

**Title rules:**
- 4–6 words. Try hard not to wrap to two lines.
- Sentence case. No period. No exclamation point.
- Do NOT use "New:" as a prefix. Instead of "New: Returns dashboard," try "A new way to manage returns."

**Body copy rules:**
- 2–4 sentences. Lead with what changed or what's now possible, then connect to workflow value.
- Do not restate the title. First sentence adds new information.
- Tell, don't sell. Lead with the workflow change, not the wow factor.
- Be specific. Vague copy like "a better way to manage your documents" is not acceptable.
- Do not explain how to use the feature in detail — that belongs in a step-through or Help documentation.

**Anchor text:** Optional. Use when a Help article adds value. "Learn more" is not sufficient — use a descriptive label.

**Button labels:**
- Primary: Specific verb matching the next available action. "Browse templates," "Start the tour," "See what's changed."
- Do NOT use "Got it" or "OK" — these close the moment instead of extending it.
- Secondary: Only present if the primary button launches a tutorial. Use "Skip" if the tutorial is not in the Guidance Hub; "Maybe later" if it can be launched there.

**Structural specs:**
- Width: 548 px
- Text alignment: left
- Optional image (min 500×200 px, max 500×500 px) or no image
- Bell icon
- Overlay: #000000 at 30% (dialog), or flexible width at top of page (embedded)

---

## Major Announcement (Megaphone/Bullhorn icon)

**When to use:** Significant product or platform moments beyond a feature update. Major releases, community events, high-value webinars, org-wide communications with broad user relevance. If the news wouldn't register as a significant moment for most users, use Feature Announcement instead.

**Voice and tone:** Passionate (frame the moment — specific, energizing, workflow-oriented). Confident (direct, specific, present tense).

**Title rules:**
- Frame the significance of the moment, not just the name of the thing. "Ready to Review is here" ✅ / "Introducing Ready to Review" ❌
- 4–6 words. Try hard not to wrap to two lines.
- Sentence case. No period. One exclamation point permitted only if the moment genuinely warrants it.

**Body copy rules:**
- 2–4 sentences. Lead with what changed or what's now possible, then connect to workflow value.
- Do not restate the title.
- More latitude for "we" framing than Feature Announcement — appropriate for moments where TR is making a meaningful commitment.
- Passionate ≠ marketing language. Passionate is specific and action-oriented. Marketing language is vague and self-congratulatory.
- If announcement has scope/eligibility constraints (beta, admin only, specific tier), surface them in the body. Don't let users discover the limitation on their own.

**Anchor text:** Optional. Use for registration links, release notes, or resources that add direct value. Label specifically.

**Button labels:**
- Primary: Specific verb reflecting the most valuable action. "Watch the webinar," "Start the tour," "Join the community."
- Secondary: Customizable.

**Structural specs:** Same as Feature Announcement (548 px, left-aligned, megaphone icon).

---

## Step-through Tutorial (Circle-info icon, anchored popover)

**When to use:** A multi-step guided walkthrough anchored to specific UI elements. Demonstrates a new feature workflow or helps users build confidence with a non-obvious interaction. Each step corresponds to something visible or interactive on screen. Can be triggered from a feature announcement.

**Voice and tone:** Confident (respect the user's expertise, keep momentum). Precise (one idea per guide, nothing more). No marketing language or platitudes.

**Title rules:**
- 3–5 words. Should not wrap to a second line.
- Sentence case. No period.
- Use unique titles for each step that summarize the key benefit (e.g., "Import data faster").

**Body copy rules:**
- 1–3 sentences. Never more than 1 paragraph.
- Describe what the user is seeing and why it matters in the context of their workflow.
- Do not explain domain concepts the audience already knows.
- Do not attempt to document every option or setting visible on screen.

**Step count and sequence:**
- Aim for 3–6 steps. Data trends indicate steep drop-off after 4 guides. More than 6 suggests the feature scope may need review.
- Steps should be sequenced in the order a user would actually encounter them.

**Anchor text:** Use sparingly. Keeps the user in-app. Appropriate only when a step references a specific Help article that adds direct value. "Learn more" is not sufficient.

**Button labels:**
- Standard labels: Back, Next, Done.
- Do NOT include Back on the first step.

**Structural specs:**
- Dialog width: 548 px
- Text alignment: left
- Circle-info icon
- Step counter: "Step N of N"
- Optional image (min 500×200 px, max 500×500 px) or video
- Overlay: #000000 at 30%

---

## Contextual Guide / Tooltip (Circle-info popover, no overlay)

**When to use:** Attached to a specific UI element. Triggered by user interaction (field focus, hover, page load). Used to clarify non-obvious UI behavior, surface constraints, or provide just-in-time information. Not for feature announcements or onboarding. No CTA — dismiss only. If the moment requires the user to take action, use a different template.

**Voice and tone:** Precise only. Contextual guides fire mid-task. No room for anything extra. Omit articles where natural. Descriptive, specific verbs. No hedging, no warmth padding. Most actionable detail comes first. Genuine and Passionate have no place here.

**Title rules:**
- 1–4 words. Shares a line with icon and × — shorter is better.
- Sentence case. No period.

**Body copy rules:**
- 1–2 sentences. Lead with what the user needs to know to act correctly on this element.
- Write for the gap between what the label says and what the user needs to know. If the element is self-evident from its label, a contextual guide probably isn't needed.
- State constraints, defaults, or downstream effects if relevant.

**Anchor text:** Do not use. If supplemental information is truly required, use a different template.

**Button labels:** Close (X) only. No CTA.

**Structural specs:**
- Width: 232 px
- Contains Close (X) button
- Text length: up to 40 words of plain text, rich text, or HTML markup, plus optional title

---

## Feedback Survey (Message-dots icon)

**When to use:** Collecting satisfaction ratings and optional qualitative feedback on a specific product or feature. Delivered as a two-screen sequence: survey screen followed by confirmation screen.

**Voice and tone:** Genuine. Natural, plain language, no formality. The thank-you screen in particular should feel like a real acknowledgment, not a system confirmation. Avoid Precise here — clinical copy creates distance at exactly the wrong time.

**Title and button labels:** Fixed. Do not edit.

**Rating question:** Replace [product or feature] with the specific product or feature name exactly as it appears in the UI. Use the exact label — not a description, not an informal name. Do not rewrite "How satisfied are you with."

**Open text question:** The default ("What influenced your rating?") works well. Don't replace without a clear reason. Do not ask multiple questions. Always optional.

**Thank you message:** Replace [product or feature] consistently. Keep short. Don't embellish "Your input helps make [product or feature] better."

**Anchor text:** Optional. Use when there's a relevant next step — resource, community link, or related feature.

**Structural specs:**
- Width: 548 px
- Text alignment: left
- Message-dots icon

---

## Warning (Triangle-exclamation icon)

**When to use:** Planned outage for maintenance or unforeseen service degradation.

**Options:**
- Dialog (Option 1): Modal overlay for warnings that cannot be missed
- Embedded guide (Option 2): Non-interruptive, at top of page

**Structural specs:**
- Dialog width: 548 px
- Overlay: #000000 at 30%
- Use Attention icon (triangle-exclamation)
- Image: min 500×200 px, max 500×500 px
- Embedded: Flexible width, top of page, Close (X) button

**Button labels (Dialog):**
- Secondary: descriptive (not "Label text")
- Primary: "I acknowledge" is acceptable for warnings

---

## Completion Step (Circle-check icon)

**When to use:** Final step of a walkthrough to confirm completion and optionally link to next steps.

**Structural specs:**
- Simple dialog, no image
- Dialog width: 548 px
- Text alignment: left
- Circle-check (Confirmation) icon
- Overlay: #000000 at 30%
- Can remove icon/link/secondary button if needed

**Button labels:**
- "Got it!" is acceptable on this specific template only.
- Optional secondary button (e.g., "Cancel") only if needed.

---

## Polls (Embedded in tutorial or standalone)

**Poll types:** Number scale, open text, multi-choice (radio or dropdown), Yes/No

**Structural specs:**
- Width: 548 px (except number scale: flexible)
- Text alignment: left
- Message-dots icon
- Overlay: #000000 at 30%
- Can remove icon/link/secondary button

---

## Resource Center

**Modules:** Guide List, Onboarding, Announcement, Sandbox, External website

**Not a guide type in itself** — it's a container. Review the individual modules inside it using the rules for the guide types they surface.
