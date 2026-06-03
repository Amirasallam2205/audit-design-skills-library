# Error Message Patterns Reference

All patterns sourced from Thomson Reuters UX Content Standards. Apply the matching pattern for the classified error type. Use exact pattern structure; fill in `<placeholders>` with real content from context.

---

## Field Validation (inline, under form fields)

Appear under the affected field after a failed submission attempt. Tell the user what to fix and how.

| Scenario | Pattern | Example |
|----------|---------|---------|
| Missing info (standard) | Enter a/an/your [field name]. | Enter your last name. |
| Missing info (alternate/complex label) | *contextual* | Confirm your password to continue. |
| Wrong format | Use the format [format]. | Use the format MM/DD/YYYY. |
| Incorrect or unrecognized | Unrecognized [item]. | Unrecognized promo code. |
| Expired | [Item] has expired. | Discount code has expired. |
| Duplicate | [Label] is already in use. Enter a different [label]. | File name is already in use. Enter a different name. |
| Can't contain certain characters | [Label] can't contain [character type]. | Cities can't contain numbers. |
| Can contain only certain characters | [Label] can contain only [character type]. | Account ID can contain only numbers. |
| Character count too few | [Label] must be [n] characters or more. | Passwords must be 9 characters or more. |
| Character count exact | [Label] must be [n] [character type]. | Phone number must be 10 digits. |
| Character count range | [Label] must be between [n] and [n] characters. | PINs must be between 4 and 6 characters. |
| Character count too many | [Label] must be [n] characters or fewer. | Usernames must be 20 characters or fewer. |
| Illogical dates | [Label] must be/can't be [before/after/on or after] [reference date]. | Start date must be before end date. |
| Mismatched fields | Both [labels] must match. | Both passwords must match. |
| Unsupported file type | File must be [list of valid types]. | File type must be PDF, DOC, or CSV. |
| File too large (single) | File can't exceed [n MB]. | File can't exceed 25 MB. |
| File too large (total) | Files can't exceed [n MB] total. | Files can't exceed 50 MB total. |
| Input exceeds logical maximum | [Field] cannot exceed [other item or amount]. | Number of periods cannot exceed number of days in fiscal year. |
| Incomplete task / blocked next step | [Do something]. / [Do something] to continue. / [Do something] to [perform action]. | Select at least one request type. Upload your signature to continue. |
| Incorrect login | Make sure your [identifier] and password are correct. / Incorrect [identifier] and/or password. | Make sure your email and password are correct. |
| Password field — fields must match | Passwords must match. | Passwords must match. |
| Password required | Password is required. | Password is required. |

---

## Form Banner (top-of-form inline alert)

Appears when 3+ fields fail validation simultaneously. Pulls keyboard/focus to top.

| Scenario | Pattern | Example |
|----------|---------|---------|
| Multiple field errors | To continue, fix the [n] issues identified on this form. | To continue, fix the 3 issues identified on this form. |
| Single field error (banner still used) | To continue, fix the issue identified on this form. | To continue, fix the issue identified on this form. |

> **Note:** Short forms (1–3 fields) do not require an error banner.

---

## System Errors

Appear as toasts, modals, or banner alerts when something fails on the backend.

### Identifiable system error (cause known)

| Pattern | Example |
|---------|---------|
| We couldn't [attempted action]. Try [remedy]. | We couldn't attach your file. Try refreshing the page. |

### Unknown system error (cause unclear, remedy known)

| Pattern | Example |
|---------|---------|
| Something went wrong. Try [remedy]. | Something went wrong. Try refreshing the page. |

### Unknown system error (generic fallback)

| Pattern | Example |
|---------|---------|
| Something went wrong. Try [suggestion]. If the problem continues, contact Support. | Something went wrong. Try again in a moment, or contact Support if the problem continues. |

---

## Timeout / Session Errors

### Session timeout (Error 401)

| Pattern | Example |
|---------|---------|
| Your session has timed out. Please sign in again. | Your session has expired. Please sign in again. |

> "Please" is acceptable here — this is an inconvenience caused by the system, not the user.

---

## Permission / Access Errors

### Permission denied (Error 403)

| Pattern | Example |
|---------|---------|
| You need [permission/a license] to access this [product/content]. Contact [name] for help. | You need permission to access this engagement. Contact your administrator for help. |

---

## Not Found Errors

### Page not found (Error 404)

| Pattern | Example |
|---------|---------|
| We can't find this page. Maybe one of these links will help: [link 1], [link 2] | We can't find this page. Maybe one of these links will help: Contact Support, TR.com |

---

## Server Errors

### Unspecified server error (Error 500)

| Pattern | Example |
|---------|---------|
| There was an issue processing your request. Try again, or contact Support if the problem continues. | There was an issue processing your request. Try again, or contact Support if the problem continues. |

---

## File Upload Errors

| Scenario | Pattern | Example |
|----------|---------|---------|
| Unsupported file type | [Filename] could not be uploaded. File type must be [PDF, DOC, etc.]. | Document.eml could not be uploaded. File type must be PDF, DOC, or CSV. |
| File too large | File can't exceed [n MB]. | File can't exceed 25 MB. |
| Generic upload failure | We couldn't upload your file. Try again. | We couldn't upload your file. Try again. |

---

## Registration Errors

| Scenario | Pattern | Example |
|----------|---------|---------|
| Already registered | You already registered for [product]. Want to sign in? | You already registered for Onvio. Want to sign in? |
| Email verification failed | Something isn't right. Return to the email and [best suggestion]. | Something isn't right. Return to the email and try the Verify button, or be sure you're copying and pasting the entire link. |

---

## Document Retrieval Errors

| Pattern | Example |
|---------|---------|
| There's a temporary issue accessing your [document]. Try again in a little while. | There's a temporary issue accessing your return. Try again in a little while. |

---

## Alert Type Reference

Use this to determine the correct visual treatment alongside copy:

| Alert color | When to use | Tone notes |
|-------------|-------------|------------|
| **Red (error)** | Something outside the user's control has failed | Avoid "fail/failure"; "please/sorry" OK if system is at fault |
| **Yellow (warning)** | User needs to know something critical about an action they've taken or will take | Avoid "you/your" when it could sound accusatory; frame as opportunity |

**Alert hierarchy** (when stacking multiple alerts):
1. Error
2. Warning
3. Informational
4. Success

---

## Banned words — never use

- `invalid`
- `fatal`
- `forbidden`
- `fail` / `failure`
- `you` / `your` when it could appear to blame the user

## "Please" and "sorry" — use sparingly

Only when:
- The failure is on our side (system malfunction, no user recovery path)
- The user is genuinely inconvenienced through no fault of their own

Never use them for user-caused input errors.

---

## Abbreviation rules (relevant to error messages)

- File types in ALL CAPS when referencing the type: `PDF`, `DOCX`, `CSV`
- File types in lowercase when part of a filename: `budget_template.xlsx`
- File sizes with a space: `25 MB` (not `25MB`)
- Common shortenings OK: `admin`, `app`, `info`
- No texting slang or internet abbreviations
