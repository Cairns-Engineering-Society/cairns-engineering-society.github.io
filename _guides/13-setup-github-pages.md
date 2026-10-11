# 13 – Setting up GitHub Pages (one time only)

How the website was switched on, and the placeholders that still need to be filled in. You only need this guide when the site is first launched, or if the site ever stops appearing.

---

## Turning the website on

**Only the CES GitHub account can do this.**

1. Sign in to GitHub **as the CES account** (`cairns-engineering-society`).
2. Go to the repository: https://github.com/cairns-engineering-society/cairns-engineering-society.github.io
3. Click **Settings** → in the left menu, click **Pages**.
4. Under **Build and deployment**:
   - **Source:** `Deploy from a branch`
   - **Branch:** `main` and folder `/ (root)`, then click **Save**.
5. Wait 1–2 minutes and refresh the Settings → Pages screen. It should say **"Your site is live at https://cairns-engineering-society.github.io"**.
6. Also on that page: if there is an **Enforce HTTPS** tick box, make sure it's ticked.

Why this name works: a repository named exactly `<account-name>.github.io` becomes that account's main website. **Never rename the repository or the CES account**, or the website address will change.

## Filling in the placeholders

Anything not known when the site was built is marked **PLACEHOLDER**. To find them all:

1. On the repository's main page, press `/` (or click the search box at the top).
2. Type `PLACEHOLDER` and press Enter. GitHub lists every file and line containing it.

| Placeholder | What goes there | Guide |
|---|---|---|
| ~~Calendar embed and subscribe links~~ | ✅ Done October 2026 | [11](11-setup-google-calendar.md) |
| ~~Google Form links~~ (suggestions, event suggestions, subject review, testimonial) | ✅ Done October 2026 | [12](12-setup-google-forms.md) |
| ~~Constitution PDF~~ | ✅ Done October 2026 (`files/CES-Constitution.pdf`) | [03](03-uploading-a-file.md) |
| `[PLACEHOLDER: ...]` text on pages | Real content: committee names, placement steps, links, etc. | [01](01-editing-a-page.md) |

Search only looks at the `main` branch and may take a few minutes to include brand-new changes.

## Before telling students about the site

- [ ] No `PLACEHOLDER` text visible on the live site's main pages.
- [ ] Calendar shows on the home page, and both subscribe links and the QR code work.
- [ ] Every link on the home page opens the right page, and every "← Back to home" link works.
- [ ] Constitution PDF opens from the Documents page.
- [ ] Placement page checked against the official documents (and ideally by the placement coordinator).
- [ ] Checked on a phone as well as a computer.

## If the site ever disappears

1. Check **Settings → Pages** (as the CES account) still says the site is live, and the source is still `main` / `(root)`.
2. Check the **Actions** tab for a ❌ red cross. See [08 – Undoing a mistake](08-undoing-a-mistake.md).
3. Check nobody renamed the repository or the account.
