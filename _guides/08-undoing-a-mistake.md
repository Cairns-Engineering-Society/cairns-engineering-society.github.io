# 08 – Undoing a mistake

**Don't panic.** GitHub keeps every version of every file forever. Whatever happened, it can be put back.

---

## How do I know something broke?

- The page on the live site looks wrong (tables showing as `|` characters, missing sections, etc.).
- Or the site didn't update. Go to the repository and click the **Actions** tab. Each save creates a "pages build and deployment" entry:
  - ✅ green tick = worked
  - 🟡 yellow dot = still updating, wait a minute
  - ❌ red cross = failed, and the live site is still showing the last version that worked

## Fix 1: Just edit it again (most common)

Most problems are a small formatting slip. Open the file, compare it to the template or the [Markdown cheat sheet](07-markdown-cheat-sheet.md), fix it, and commit. Common causes:

- a missing **blank line** (before a heading, list, table, or after `</summary>`)
- a blank line **inside** a table
- a missing `)` or `]` in a link
- a missing `</details>` on a subject page

## Fix 2: Put a file back to an earlier version

Use this when you're not sure what went wrong and just want the old version back.

1. Open the file on github.com.
2. Click **History** (the clock icon, near the top right of the file). You'll see a list of every change, newest first, with who made it and when.
3. Find the last version that was correct (the change **before** the mistake). On that row, click the **`<>`** button ("Browse repository at this point in the history").
4. You're now looking at the whole site as it was back then. Click through to the same file (e.g. `events.md`, or `subjects` → `level-1.md`). This is the old version. Click the **Raw** button (or the copy icon ⧉ "Copy raw file").
5. Copy **all** of the text (**Ctrl+A** then **Ctrl+C**, or **Cmd+A** then **Cmd+C** on a Mac).
6. Go back to the **current** version of the file (click the repository name at the top, then the file), and click the pencil icon ✏️.
7. Select all the text in the editor and paste over it.
8. Commit with a message like `Restore events page to version from 10 Oct`.

## Fix 3: Get back a deleted file

1. Go to the repository's main page and click the **commits** link (it shows a number with a clock icon, near the top of the file list).
2. Find the commit that says the file was deleted, e.g. "Delete events.md".
3. On the row **just below it** (the change before the deletion), click the **`<>`** button ("Browse repository at this point in the history"), then click the file to open it.
4. Copy its text (Raw → select all → copy), then recreate the file with **Add file → Create new file** using the exact same name, paste, and commit.
5. For deleted PDFs or images: download the old file from that earlier version (the **download** button ⬇) and upload it again.

---

## Still stuck?

- Ask another committee member who has edited the site before.
- Leave it as it is. The live site keeps showing the last working version if an update fails, so nothing breaks for students while you get help.
