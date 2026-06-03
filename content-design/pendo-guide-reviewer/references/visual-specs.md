# Visual and Structural Specs Reference

Sourced from TR Pendo Guides Library (Figma). Apply these when checking structural compliance.

---

## Dialog dimensions

| Guide type | Width | Notes |
|---|---|---|
| Standard dialog (most types) | 548 px | Feature announcement, announcement, tutorial, warning, completion, polls |
| Tooltip / popover | 232 px | Contextual guide only |
| Embedded guide | Flexible | Full width at top of page |

---

## Text alignment

All guide types: **left-aligned**.

---

## Overlay (modal dialogs)

Background: **#000000 at 30% opacity**

Applies to: Feature announcements, major announcements, tutorials, warnings, polls, completion steps, dialogs with images.

Does NOT apply to: Embedded guides (no overlay).

---

## Icon mapping

| Icon name | Guide type |
|---|---|
| Bell (bell) | Feature announcement |
| Megaphone/bullhorn (bullhorn) | Major announcement, events, recruiting |
| Circle-info (circle-info) | Tutorial, informational, contextual |
| Triangle-exclamation | Warning |
| Circle-check | Completion / confirmation |
| Circle-question | Support / "Have a question?" |
| Message-dots | Feedback / polls |

---

## Image specs

| Context | Min size | Max size |
|---|---|---|
| Standard dialog with image | 500×200 px | 500×500 px |
| Announcement 1.2 (image-led layout) | 548×240 px | — |

Images are optional on most templates. You can remove image/icon/link/secondary button as needed.

---

## Step counter format

**Tutorial only:** "Step N of N" — appears below the title, above body copy.

---

## Close button

All guide types must include a Close (X) button.

---

## Embedded guide placement

- Place at **top of page**
- Flexible width
- Contains Close (X) button
- Appears when user reopens the application
- User must close it manually

---

## Popover / tooltip specs

- Width: 232 px
- Contains Close (X) button
- Text: up to 40 words plain text, rich text, or HTML + optional title
- Activates/closes when clicking on the triggering element

---

## Overlay (modal) behavior

- Overlay in center of screen
- Background: #000000 at 30%
- Standard for Feature announcements, walkthroughs, warnings, polls

---

## Resource Center visual specs

- Header: TR orange accent bar at top
- Contains: Guide List module, Onboarding module, Announcement module, Sandbox module, External website module
- Each module shows title + subtitle with right-pointing chevron
- Close (X) button top right
- Individual sub-views: back-arrow (chevron-left) + module title + Close (X)

---

## Announcement variants

### Feature Announcement
- **1.1** — Simple dialog with image: bell icon + title + body + image + optional link + optional secondary + primary CTA
- **1.2** — Image-led: large image at top + bell icon below + title + body + primary CTA only (548×240 px image)
- **2** — Embedded guide: no overlay, flexible width, top of page

### Major Announcement  
Same variants as Feature Announcement but with megaphone icon.

---

## Event/Promotion variants

- **1.1** — Simple dialog with image (bullhorn icon)
- **1.2** — Image-led dialog (bullhorn icon, 548×240 px)
- **2.1** — Embedded guide, standard
- **2.2 (Big)** — Embedded banner with image, max 3 lines of text including link
- **2.2 (Small)** — Embedded banner, max 2 lines of text including link

---

## Completion step

- Simple dialog, no image
- Dialog width: 548 px
- Circle-check icon
- "Got it!" is the correct primary button label for this template only

---

## Poll variants

| Poll type | Width |
|---|---|
| Number scale | Flexible |
| Open text | 548 px |
| Multi-choice (radio) | 548 px |
| Multi-choice (dropdown) | 548 px |
| Yes/No | 548 px |
