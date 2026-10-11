# 12 – Google Forms (done, and how to redo them)

Four Google Forms let students contribute **without needing GitHub**. The committee reviews the responses and copies the good ones onto the site. **All four are already set up and linked from the site** (October 2026).

| Form | Link | Linked from | Responses used in |
|---|---|---|---|
| **Suggest something for the CES website** | https://forms.gle/n4fg7VV2BTVFQaYu6 | Every page footer, the home page, About, Placement, Things nobody tells you | Fixing and improving any page |
| **Review a subject** | https://forms.gle/J5Wc61eYJdNEJ3gW7 | Subjects pages (every subject dropdown) | [04 – Adding a subject](04-adding-a-subject.md) |
| **Share your experience** (testimonial) | https://forms.gle/UomxoXyUfCtqANSL6 | Testimonials page | [05 – Adding a testimonial](05-adding-a-testimonial.md) |
| **Suggest an event** | https://forms.gle/sGoZM1dob3ePv7Xd8 | Events page | Planning events at committee meetings |

All four forms and their response spreadsheets belong to the CES Google account (`cairns.engineering.society@gmail.com`).

**Changing a question?** Edit the form in Google Forms. The link stays the same, so you don't need to touch the website.

**When a new major starts** (e.g. Civil in Cairns), add it to the "Your major" question in the subject review and testimonial forms.

The rest of this guide is only needed if a form ever has to be **made again from scratch**.

---

## Creating a form

1. Sign in to [forms.google.com](https://forms.google.com) **as the CES Google account**. The forms and responses must belong to CES, not a personal account, so they survive committee changes.
2. Click **Blank form** (the big **+**).
3. Give it a title and add the questions below. Click **+** on the right to add each question and choose its type from the drop-down.
4. **Responses** tab → **Link to Sheets** → **Create a new spreadsheet**. All responses then go into a Google Sheet that's easy to read.
5. **Settings** tab → **Responses** → leave **Collect email addresses** set to **Do not collect**, unless you specifically want emails.
6. Click **Send** (top right) → the **link** icon 🔗 → tick **Shorten URL** → **Copy**. That's the link for the website.

## Form 1: Suggestions

Title: **Suggest something for the CES website**
Description: *Spotted a mistake, or know something that should be on the site? Let us know.*

| Question | Type | Required? |
|---|---|---|
| What's your suggestion or correction? | Paragraph | ✅ |
| Which page is it about? (if any) | Short answer | |
| Can we contact you about it? If so, how? | Short answer | |

## Form 2: Subject review

Title: **Review a subject**
Description: *Help the next group of students know what to expect. Reviews are checked by the CES committee before being added to the website.*

| Question | Type | Required? |
|---|---|---|
| Subject code (e.g. EG1000) | Short answer | ✅ |
| Subject name | Short answer | |
| When did you take it? (e.g. Trimester 1, 2026) | Short answer | ✅ |
| Your major | Multiple choice: Electrical / IoT / Mechanical / Maritime / Other | ✅ |
| What was the subject actually like? | Paragraph | ✅ |
| Workload | Multiple choice: Light / Moderate / Heavy | ✅ |
| What was the assessment like? | Paragraph | |
| Any tips for future students? | Paragraph | |
| How should we credit you? | Multiple choice: "First name only" / "Year only (e.g. 2026 student)" / "Don't credit me" | ✅ |
| First name (only if you chose "First name only") | Short answer | |
| I agree that CES may publish my review (possibly edited for length) on the public CES website. | Checkboxes (one box) | ✅ |

## Form 3: Testimonial

Title: **Share your experience**
Description: *Tell future students about your engineering degree, placement or CES experience.*

| Question | Type | Required? |
|---|---|---|
| Your testimonial | Paragraph | ✅ |
| Your major | Multiple choice: Electrical / IoT / Mechanical / Maritime / Other | ✅ |
| Where are you up to? (e.g. 3rd year, Graduated 2025) | Short answer | ✅ |
| How should we credit you? | Multiple choice: "First name" / "Anonymous" | ✅ |
| First name (only if you chose "First name") | Short answer | |
| I agree that CES may publish this on the public CES website. | Checkboxes (one box) | ✅ |

## Form 4: Event suggestions

Title: **Suggest an event**
Description: *Is there an event you'd like CES to run? Tell us your idea. The committee reads every suggestion when planning each trimester.*

| Question | Type | Required? |
|---|---|---|
| What event would you like CES to run? | Paragraph | ✅ |
| What type of event is it? | Multiple choice: Social / Industry or careers / Study or academic / Other | ✅ |
| When would suit you best? | Checkboxes: Weekday daytime / Weekday evening / Weekend | |
| Roughly how much would you pay to attend? | Multiple choice: Only if it's free / Up to $5 / Up to $10 / Up to $20 / More than $20 | |
| Would you be keen to help organise it? | Multiple choice: Yes / Maybe / No | |
| If yes or maybe, how can we contact you? | Short answer | |

## If a form is made again: update the links

A new form has a new link, so every place the old link appears needs updating:

1. On the repository's main page, press `/` and search for the end part of the **old** link (e.g. `n4fg7VV2BTVFQaYu6`). GitHub lists every file containing it.
2. For each file: open it, click the pencil icon ✏️, press **Ctrl+F** (**Cmd+F** on a Mac) to find each copy of the old link, replace it with the new link, then commit.
3. Repeat the search until it finds nothing.
4. Update the table at the top of this guide.

The suggestions form link is also in the footer of [`_templates/new-page.md`](../_templates/new-page.md), and the subject review link is in [`_templates/new-subject.md`](../_templates/new-subject.md). The search finds those too.

## Checking responses

- Open the linked Google Sheet (or the form's **Responses** tab) every few weeks.
- Turn on email alerts: **Responses** tab → **⋮** → **Get email notifications for new responses**.
- Add good responses to the site using [04 – Adding a subject](04-adding-a-subject.md) or [05 – Adding a testimonial](05-adding-a-testimonial.md).
