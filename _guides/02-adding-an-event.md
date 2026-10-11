# 02 – Adding an event

Events live in two places, and each has a different job:

| Where | What goes there | When |
|---|---|---|
| **The CES Google Calendar** (shown on the home page) | **Upcoming** events with dates, times, places and sign-up links | **Before** the event |
| **The Events page** (`events.md`) | An overview of what CES does: **regular events** and a record of **past events** | **After** the event, or when CES starts or stops a regular event |

The Events page deliberately doesn't list upcoming dates. Keeping dates only in the calendar means there's one place to update, and the site can't show two different times for the same event.

---

## Part A: Add an upcoming event (Google Calendar only)

**Time:** about 2 minutes. No GitHub needed.

1. Sign in to [calendar.google.com](https://calendar.google.com) with the **CES Google account** (`cairns.engineering.society@gmail.com`), or your own account if the CES Events calendar has been shared with you with "Make changes to events" permission.
2. Click the date of the event, then **More options**.
3. Fill in the **title**, **time** and **location**. In the description, add details such as cost, what to bring and the sign-up link.
4. **Important:** check the calendar drop-down (near the bottom, usually shows a coloured dot and a calendar name) is set to **CES Events**, NOT the account's main calendar. Otherwise it won't appear on the website.
5. Click **Save**.

The home page calendar and everyone who subscribed get the event automatically within a few minutes.

**Changing or cancelling:** open the event in Google Calendar and edit or delete it. If you cancel, consider renaming it `CANCELLED – [event name]` for a day or two before deleting it, so people who saw it know.

## Part B: Record a past event (Events page)

**Time:** about 3 minutes. Do this after the event, or once at the end of each trimester for all of that trimester's events.

1. Open [`_templates/new-past-event.md`](../_templates/new-past-event.md) and copy the template line.
2. Open `events.md` and click the pencil icon ✏️ (see [01 – Editing a page](01-editing-a-page.md)).
3. Scroll to **Past events** and find the heading for this year (e.g. `### 2026`). If there isn't one, add it **above** the older years, with a blank line before and after.
4. Paste the line **directly under the year heading** (newest at the top) and replace the `[...]` parts.
5. Click **Commit changes...**, write a message like `Add T3 movie night to past events`, and click **Commit changes**.

## Part C: Add, change or remove a regular event (Events page)

The **Our regular events** section describes the events CES runs again and again (currently BBQs, movie and pizza nights, bowling and roller skating, and end of trimester events in Trimesters 2 and 3).

- **Change a description:** edit the text under its `###` heading, e.g. if the BBQ location changes.
- **Add a new regular event:** copy the block from [`_templates/new-regular-event.md`](../_templates/new-regular-event.md) and paste it at the end of the section, just above `## Suggest an event`.
- **Remove one CES no longer runs:** delete its `###` heading and description.

Then commit as usual.

## Check it worked

After 1–2 minutes, open the live Events page and check your change. Headings should appear as headings, and past events as bullet points.

---

## Event suggestions from students

The **Suggest an event** link on the Events page goes to the **event suggestions Google Form**. Responses go to a Google Sheet in the CES Google account. Look through it at committee meetings when planning the next trimester. See [12 – Setting up Google Forms](12-setup-google-forms.md).
