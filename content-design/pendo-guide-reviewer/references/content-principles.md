# Content Principles Reference

All UX content — including error messages — must be considered, concise, compelling, consistent, and correct. Apply these principles when writing and self-checking every message.

---

## The 5 Cs

### Considered
Content should be empathetic, inclusive, relevant, and user-centered.

- Put the most important info first
- Speak to the user's goal, not the UI
- Use plain language
- Contextualize content based on where the user is in their journey
- Avoid exclusionary language (no directional words like top, bottom, left, right)

### Concise
Content should be easy to scan and contain just enough words.

- Choose simple words
- Write short sentences
- Don't overload the user with too much info at once
- Remember content will be translated — keep it tight

| Do | Don't |
|----|-------|
| Enter your email. | Please enter your email address. |
| There was a server error. Try again. | A problem occurred at the server level; please try again. |

### Compelling
Content should be engaging, trustworthy, and helpful.

- Seek to move the user forward
- Use active voice as much as possible
- Avoid jargon, idioms, metaphors, and words that take effort to understand

### Consistent
Content should be standardized within and across products.

- Use repeatable content models whenever appropriate
- Don't sacrifice usability to force consistency

### Correct
Content should be accurate and use the right punctuation, grammar, and voice.

- Adhere to relevant conventions in these standards
- Use the right pattern for the error type (see `patterns.md`)

---

## Voice and tone

### Active voice (default)
Use active voice to create a clear, strong tone.

**Exceptions — use passive voice when:**
- Avoiding blaming an error on the user
- The subject is not clear
- It's more important to emphasize the action than who does it

| Do | Don't |
|----|-------|
| We couldn't save your changes. | Your changes weren't saved by the system. |
| Your session has expired. | The session was expired. |

### Errors specifically
Error alerts should always aim to use active voice — but passive voice is acceptable when it shifts blame away from the user.

---

## Grammar

### Pronouns
- Use **you / your** to address the user directly
- Use **they / them** as a singular pronoun when gender is unknown
- Use **we / our** when referring to the system or company (e.g., "We couldn't load your file")
- Avoid **me / my / I** — don't take the user's point of view
- Avoid gendered pronouns (he/she, his/her) unless referring to a specific named person

### Omit "that"
The word "that" can usually be removed for conciseness.

| Do | Don't |
|----|-------|
| Select the file you want to upload | Select the file that you want to upload |

### Articles
Generally omit articles (a, an, the) in labels and short UI copy.

| Do | Don't |
|----|-------|
| View invoice | View an invoice |
| Select tax type | Select the tax type |

### Contractions
Use common contractions to sound conversational. Avoid colloquial or regional contractions.

---

## Punctuation

### Periods
- Use periods at the end of complete sentences in error messages
- Avoid periods in bullets, headings, buttons, and stand-alone links

### Exclamation marks
Never use in error messages or negative contexts.

### Colons
In field labels, use a colon only when the label asks the user to select, read, or do something.

### Hyphens and dashes
- Use hyphens (-) to connect 2-word compounds (e.g., sign-in, read-only)
- Use "to" instead of en dashes in ranges (e.g., 9 a.m. to 5 p.m.)
- Use em dashes (—) sparingly; insert spaces on both sides

### Oxford commas
Use the Oxford comma in a series of 3 or more items.

> Get resources for trusts, estates, labor, and employment. ✓

### Ampersands
Spell out "and" — don't use & unless it's part of a proper name or space is extremely constrained.

### Ellipses
Use the ellipsis symbol (…), not 3 periods. Avoid in placeholder text.

---

## Capitalization

- Use **sentence case** for all UI copy — capitalize only the first word and proper nouns
- Do not use title case for error messages, labels, or buttons
- Do not use ALL CAPS except for acronyms, file type extensions, and certain trademarked product names
- Boolean operators (AND, OR, NOT) are caps

| Do | Don't |
|----|-------|
| Something went wrong. Try again. | Something Went Wrong. Try Again. |
| File must be PDF, DOC, or CSV. | file must be pdf, doc, or csv. |

---

## Numbers

- Use numerical digits, not spelled-out words (3 not three)
- Use commas for 4+ digit numbers (1,000 not 1000)
- Use negative symbol for negative numbers, not parentheses
- File sizes: always include a space (25 MB not 25MB)

---

## Accessibility considerations

- Put the most important info first — screen readers read top to bottom
- Avoid orientation language (left, right, top, bottom, above, below)
- Don't rely on color alone to convey meaning
- Use plain language; avoid idioms and jargon
- Write for translation — keep sentences short and unambiguous
