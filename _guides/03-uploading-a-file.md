# 03 – Uploading a file (PDF or image)

How to put a PDF (e.g. the constitution or minutes) or an image (e.g. the calendar QR code) on the site.

**Time:** about 3 minutes

---

## Before you upload

- **Is it OK for anyone on the internet to see?** Everything uploaded here is public. Internal documents (member lists, budgets, internal minutes) go in the **CES Google Drive** instead.
- **Rename the file first, on your computer:**
  - **No spaces.** Use hyphens instead: `CES-Constitution-2025.pdf`, not `CES Constitution 2025.pdf`. Spaces cause broken links.
  - Keep it short and clear. Include the year if there will be new versions.
- **PDFs go in `files/`. Images go in `images/`.**

## Steps

1. Go to the repository: https://github.com/cairns-engineering-society/cairns-engineering-society.github.io
2. Click the **`files`** folder (for a PDF) or the **`images`** folder (for an image).
3. Click **Add file** (top right), then **Upload files**.
4. Drag your file onto the page, or click **choose your files** to find it.
5. Wait for the upload bar to finish.
6. Under "Commit changes", type a short message like `Upload 2026 AGM minutes`.
7. Click **Commit changes**.

**The file is now uploaded, but nobody can find it yet.** You need to link to it from a page.

## Link to it from a page

**For a PDF** on the Documents page: follow [`_templates/new-document.md`](../_templates/new-document.md). The link looks like this:

```
[AGM Minutes 2026](files/CES-AGM-Minutes-2026.pdf)
```

**For an image** on a page in the main folder:

```
![Description of the image for people who can't see it](images/file-name.png)
```

**Linking from a page inside `subjects/`?** Add `../` at the start, e.g. `../files/CES-Constitution-2025.pdf`.

The file name in the link must match **exactly**, including capitals and the `.pdf` / `.png` ending.

## Check it worked

After 1–2 minutes, open the page on the live site and click the link (or check the image shows). A **"404 – File not found"** page means the file name in the link doesn't exactly match the uploaded file name. Compare them letter by letter.

---

## Replacing a file with a new version

Upload the new file with the **exact same name** into the same folder. GitHub replaces the old one, and every existing link keeps working.

## Deleting a file

1. Click the file in the `files` or `images` folder.
2. Click the **⋯** (three dots) button at the top right, then **Delete file**.
3. Click **Commit changes...** and confirm.
4. **Remove any links to it** from your pages, or they'll lead to a 404 page.

## Size limits

Keep files under about **25 MB**. Large scanned PDFs can usually be shrunk with a free "compress PDF" tool. Photos straight from a phone are usually far bigger than needed, so shrink them first.
