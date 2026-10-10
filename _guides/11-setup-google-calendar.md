# 11 – Setting up the Google Calendar (one time only)

This sets up the CES events calendar shown on the home page and the "add to your phone" links. **You only do this once.** After that, adding events is just [02 – Adding an event](02-adding-an-event.md).

**Time:** about 20 minutes
**You need:** the CES Google account login, and an editor account on GitHub

---

## Part 1: Create the calendar

1. Sign in to [calendar.google.com](https://calendar.google.com) **as the CES Google account**.
2. On the left, next to **Other calendars**, click **+** → **Create new calendar**.
3. **Name:** `CES Events`. **Description:** `Cairns Engineering Society events`. **Time zone:** `(GMT+10:00) Brisbane`. Cairns is in Queensland, so there's no daylight saving.
4. Click **Create calendar**.

**Why a separate calendar?** Only events in *this* calendar will appear on the website. The CES account's own main calendar stays private.

## Part 2: Make it public

1. On the left, hover over **CES Events** → click **⋮** → **Settings and sharing**.
2. Under **Access permissions for events**, tick **Make available to public**, and make sure the drop-down says **See all event details**. Confirm the warning.

⚠️ **Everyone can now see every event in this calendar**, including descriptions. Never put private information in an event.

## Part 3: Let committee members add events (optional)

Committee members can add events from their own Google accounts instead of signing in as CES:

1. Same settings page → **Share with specific people or groups** → **Add people and groups**.
2. Add their email, set permission to **Make changes to events**, and click **Send**.

Remove people here when they leave the committee (it's on the [handover checklist](09-committee-handover.md)).

## Part 4: Get the links you need

Still on the same settings page, scroll down to **Integrate calendar**. Copy these into a note:

| What | Where to find it | Used for |
|---|---|---|
| **Embed code** | "Embed code" box (starts with `<iframe`) | The calendar on the home page |
| **Public address in iCal format** | "Public address in iCal format" (ends in `.ics`) | The iPhone/Outlook subscribe link |
| **Calendar ID** | "Calendar ID" (looks like a long email address ending `@group.calendar.google.com`) | Building the Google subscribe link |

Now make two subscribe links:

- **Google / Android link:** scroll back up to **Access permissions for events** and click **Get shareable link**. Copy the link. It looks like `https://calendar.google.com/calendar/u/0?cid=...`
- **iPhone / Outlook link:** take the iCal address and change the `https://` at the start to `webcal://`. For example, `https://calendar.google.com/calendar/ical/abc%40group.calendar.google.com/public/basic.ics` becomes `webcal://calendar.google.com/calendar/ical/abc%40group.calendar.google.com/public/basic.ics`. On iPhones and Macs, `webcal://` opens a "Subscribe?" prompt automatically.

## Part 5: Put the calendar on the home page

1. On GitHub, open `index.md` and click the pencil icon ✏️ (see [01 – Editing a page](01-editing-a-page.md)).
2. Find the **## Calendar** section.
3. Delete the line `*Calendar coming soon.*`
4. Paste your **embed code** on its own line where that line was, with a blank line before and after.
5. In the embed code, change `width="800"` to `width="100%"` so it fits phone screens.
6. Delete the whole grey `<!-- CALENDAR SETUP ... -->` note below it, including the old placeholder iframe inside it. You don't need it anymore.

**Tip:** on phones, a list view is easier to read than a month grid. To use it, add `&mode=AGENDA` just before the closing `"` of the `src="..."` part of the embed code.

## Part 6: Put in the subscribe links

Still in `index.md`, under **### Add the CES calendar to your phone**:

1. Replace `PLACEHOLDER-GOOGLE-CALENDAR-SUBSCRIBE-LINK` with the **Google / Android link**.
2. Replace `PLACEHOLDER-WEBCAL-LINK` with the **iPhone / Outlook link** (the `webcal://` one).
3. Commit.

## Part 7: Make the QR code

The QR code lets people subscribe by scanning a poster or a slide.

1. Use any **free QR code generator** to make a QR code for the **Google / Android subscribe link**.
   ⚠️ Avoid sites offering "dynamic" QR codes or free trials. Many of them **stop working after a trial period**. You want a plain **static** QR code that you download as an image.
2. Download it as a **PNG** and rename it `calendar-qr.png`.
3. Upload it into the `images/` folder (see [03 – Uploading a file](03-uploading-a-file.md)).
4. Open `index.md`. Find the grey `<!-- QR CODE: ... -->` note, move the `![Scan this QR code...](images/calendar-qr.png)` line **out of it** (put it just above the note), and delete the rest of the note.
5. Commit.

The same image can go on posters and slides. It never needs to change, because the link never changes.

## Check it worked

After 1–2 minutes, open the live home page. You should see the calendar and the two working links. Scan the QR code with your phone to test it. Add a test event in Google Calendar, check it appears on the site within a few minutes, then delete it.

**Calendar says "Events from one or more calendars could not be shown here because you do not have permission"?** Part 2 (Make available to public) wasn't saved. Redo it.
