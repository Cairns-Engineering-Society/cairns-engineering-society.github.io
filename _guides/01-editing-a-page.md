# 01 – Editing a page

How to change any text on the website. Every other guide builds on this one, so read it first.

**Time:** about 2 minutes
**You need:** a GitHub account that has been added as an editor (see [10 – Adding or removing an editor](10-adding-or-removing-an-editor.md))

---

## Steps

1. **Sign in** to [github.com](https://github.com).
2. **Go to the repository:** https://github.com/cairns-engineering-society/cairns-engineering-society.github.io
3. **Click the file** for the page you want to change. The file names match the pages:

   | To change… | Click… |
   |---|---|
   | Home page | `index.md` |
   | About | `about.md` |
   | Your degree explained | `degree.md` |
   | Careers | `careers.md` |
   | Events | `events.md` |
   | Placement | `placement.md` |
   | Things nobody tells you | `things-nobody-tells-you.md` |
   | Testimonials | `testimonials.md` |
   | Useful JCU links | `resources.md` |
   | Documents | `documents.md` |
   | Subjects | the `subjects` folder, then `index.md` or `year-1.md` to `year-4.md` |

4. **Click the pencil icon** ✏️ ("Edit this file") near the top right of the file.
5. **Make your changes** in the editor. The text is Markdown. See [07 – Markdown cheat sheet](07-markdown-cheat-sheet.md) for bold, links, lists, etc.
   - Click the **Preview** tab at the top of the editor to see roughly how it will look. Click **Edit** to go back.
6. **Click the green "Commit changes..." button** (top right).
7. In the box that pops up, write a **short description** of what you changed in the "Commit message" field, e.g. `Add Trimester 3 BBQ to events`. Leave "Commit directly to the main branch" selected.
8. **Click "Commit changes"**.

## Check it worked

- Wait **1–2 minutes**, then open https://cairns-engineering-society.github.io and refresh the page. Your change should be there.
- Not showing yet? Wait another minute and refresh again. Your browser might also be showing an old copy: hold **Ctrl** (Windows) or **Cmd** (Mac) and press **R**.
- Still not showing after 5 minutes? Go to the repository and click the **Actions** tab. The top item should have a **green tick** ✅. A **red cross** ❌ means the update failed. See [08 – Undoing a mistake](08-undoing-a-mistake.md).

---

## Things to know

- **Grey text between `<!--` and `-->` is a hidden note** for editors. It never shows on the website. Leave these notes in place so the next person knows what to do.
- **Text in `[square brackets]` with the word PLACEHOLDER** is waiting for real information. Replace the whole thing, brackets included.
- **You can't break anything permanently.** Every saved version is kept forever. See [08 – Undoing a mistake](08-undoing-a-mistake.md).
- **Never put private information on the site:** no phone numbers, student IDs, personal emails or passwords. The site and this repository are public.
- **Editing on your phone:** it works in the GitHub mobile website, but it's fiddly. A computer is easier.
