# 02 – Adding an event

Events appear in **two places**, and you should update both:

1. **The CES Google Calendar.** This shows on the home page calendar and on the phones of everyone who subscribed. It updates instantly, and you don't need GitHub at all.
2. **The events table on the Events page** (`events.md`). This is a simple list with details and sign-up links.

**Time:** about 5 minutes

---

## Part A: Add it to the Google Calendar

1. Sign in to [calendar.google.com](https://calendar.google.com) with the **CES Google account** (or your own account if the CES calendar has been shared with you with "Make changes to events" permission).
2. Click the date of the event, then **More options**.
3. Fill in the **title**, **time** and **location**. In the description, add any details and the sign-up link.
4. **Important:** check the calendar drop-down (near the bottom, usually shows a coloured dot and a calendar name) is set to the **CES events calendar**, NOT a personal calendar. Otherwise it won't appear on the website.
5. Click **Save**.

The home page calendar updates by itself within a few minutes. You don't need to touch GitHub for this part.

## Part B: Add it to the Events page

1. Open [`_templates/new-event.md`](../_templates/new-event.md) and copy the template line.
2. Open `events.md` and click the pencil icon ✏️ (see [01 – Editing a page](01-editing-a-page.md)).
3. Paste the line on a new line **directly under the last row** of the "This trimester" table. **No blank line in between**, or the table breaks.
4. Replace each `[...]` with the event details.
5. If this is the first real event of the trimester, delete the example/placeholder row.
6. Click **Commit changes...**, write a message like `Add Welcome BBQ to events`, and click **Commit changes**.

## Check it worked

After 1–2 minutes, open the live Events page. Check the new row looks right and lines up with the other rows.

**Row looks broken** (e.g. it shows as plain text with `|` characters)? Usually one of these:
- There's a blank line between your row and the row above it. Delete it.
- The row has the wrong number of `|` characters. Every row needs 6.

---

## At the start of each trimester

1. Change the heading `## This trimester: ...` to the new trimester, e.g. `## This trimester: Trimester 1, 2027`.
2. Move last trimester's rows into **Past events**:
   - Under "Past events", add a heading like `### Trimester 3, 2026`.
   - Under it, paste the table header lines (`| Date | Time | Event | Where | More info / sign up |` and `|---|---|---|---|---|`) and then the old rows.
   - Delete the `*No past events recorded yet.*` line if it's there.
3. Leave the header lines (the first two lines) of the "This trimester" table in place and add the new events under them.

## Changing or cancelling an event

- **Google Calendar:** open the event and edit or delete it.
- **Events page:** edit the row. For a cancelled event, you can write `~~Event name~~ CANCELLED` to put a line through it.
