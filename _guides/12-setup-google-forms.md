# 12 – Setting up Google Forms (one time only)

Three forms let students contribute **without needing GitHub**. The committee reviews responses and copies the good ones onto the site.

| Form | Linked from | Replaces this placeholder |
|---|---|---|
| **Suggestions** | Every page footer, home page, About page | `PLACEHOLDER-SUGGESTION-FORM-LINK` |
| **Subject review** | Subject pages | `PLACEHOLDER-SUBJECT-REVIEW-FORM-LINK` |
| **Testimonial** | Testimonials page | `PLACEHOLDER-TESTIMONIAL-FORM-LINK` |

**Time:** about 30 minutes for all three
**You need:** the CES Google account login

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
| Your major | Multiple choice: Electrical / IoT / Mechanical / Other | ✅ |
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
| Your major | Multiple choice: Electrical / IoT / Mechanical / Other | ✅ |
| Where are you up to? (e.g. 3rd year, Graduated 2025) | Short answer | ✅ |
| How should we credit you? | Multiple choice: "First name" / "Anonymous" | ✅ |
| First name (only if you chose "First name") | Short answer | |
| I agree that CES may publish this on the public CES website. | Checkboxes (one box) | ✅ |

## Put the links on the site

Each placeholder appears on **several pages**, so replace every one:

1. On the repository's main page, press `/` and search for the placeholder, e.g. `PLACEHOLDER-SUGGESTION-FORM-LINK`. GitHub lists every file containing it.
2. For each file: open it, click the pencil icon ✏️, and replace the placeholder with the form link. Press **Ctrl+F** (**Cmd+F** on a Mac) to find each one in the file. Then commit.
3. Repeat the search until it finds nothing.

Don't forget the footer line in [`_templates/new-page.md`](../_templates/new-page.md), so new pages get the right link.

## Checking responses

- Open the linked Google Sheet (or the form's **Responses** tab) every few weeks.
- Turn on email alerts: **Responses** tab → **⋮** → **Get email notifications for new responses**.
- Add good responses to the site using [04 – Adding a subject](04-adding-a-subject.md) or [05 – Adding a testimonial](05-adding-a-testimonial.md).
