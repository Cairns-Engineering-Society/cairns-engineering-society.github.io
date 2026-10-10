# 06 – Adding a new page

Use this when a whole new topic needs its own page, e.g. "Study spaces" or "Dual degrees".

**Time:** about 10 minutes

---

## Steps

### 1. Create the file

1. Go to the repository: https://github.com/cairns-engineering-society/cairns-engineering-society.github.io
2. Make sure you're in the **main folder** (you can see `index.md` in the list). To put the page in the subjects section instead, click into the `subjects` folder first.
3. Click **Add file** (top right), then **Create new file**.
4. Type the **file name** in the box at the top. Rules:
   - **lowercase**, words joined with **hyphens**, ending in **`.md`**
   - ✅ `study-spaces.md`  ❌ `Study Spaces.md`  ❌ `study_spaces.txt`
   - The file name becomes the web address: `study-spaces.md` → `https://cairns-engineering-society.github.io/study-spaces.html`

### 2. Add the content

1. Open [`_templates/new-page.md`](../_templates/new-page.md) in another browser tab and copy the block.
2. Paste it into the new file.
3. Replace everything in `[square brackets]` and write your content. See [07 – Markdown cheat sheet](07-markdown-cheat-sheet.md).
4. Replace the footer line at the bottom with the footer line from any existing page, so the "Suggest a change" link is right.
5. If the page is inside `subjects/`, change the first line to `[← Back to home](../index.md)`.
6. Click **Commit changes...** → write a message like `Add study spaces page` → **Commit changes**.

### 3. Link to it (don't skip this!)

A page nobody links to is invisible. Add it to the home page:

1. Open `index.md` and click the pencil icon ✏️.
2. Under **Quick links**, add a line like this, in a sensible spot in the list:
   ```
   - [Study spaces on campus](study-spaces.md)
   ```
3. Commit.

(For a page in `subjects/`, link to it from `subjects/index.md` instead, e.g. `- [Dual degrees](dual-degrees.md)`.)

## Check it worked

After 1–2 minutes, open the live home page, click your new link, and check the "← Back to home" link works.

---

## Renaming or deleting a page

**Renaming** changes its web address, so links to the old name will break.
1. Open the file, click the pencil icon ✏️, and change the name in the file name box at the top.
2. Commit.
3. Update every link to it. To find them, type the old file name into the repository search box (press `/` on the repository page).

**Deleting:**
1. Open the file, click **⋯** (top right), then **Delete file**, and commit.
2. Remove the link from the home page.
