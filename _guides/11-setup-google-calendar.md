# 11 – Google Calendar setup (done, and how to redo it)

The home page calendar and the "add to your phone" links come from a Google Calendar called **CES Events**. **This is already set up**, so to add events, just follow [02 – Adding an event](02-adding-an-event.md).

Use this guide if you need to **change the calendar view**, **check how it's set up**, or **set it up again** (e.g. if the calendar was deleted).

---

## How it's set up now (October 2026)

| What | Setting |
|---|---|
| Owner | The CES Google account, `cairns.engineering.society@gmail.com` |
| Calendar name | **CES Events** |
| Time zone | Brisbane (Cairns has no daylight saving) |
| Public? | ✅ Yes, "See all event details". **Anything you put in a CES Events event is public.** |
| The account's main calendar | Deliberately **not** public. Only put public events in **CES Events**. |
| Calendar ID | `d9d1f1f2576f01714405e7e2301d3a6141c72bc7d1812b0f5403b1379cc56b9e@group.calendar.google.com` |
| On the website | The home page (`index.md`), under **## Calendar**, in **Agenda** view |
| Subscribe links | Under **### Add the CES calendar to your phone** on the home page |
| QR code | `images/calendar-qr.png`. It opens the Google subscribe link. Use it on posters and slides. It never needs to change unless the calendar is replaced. |

## Giving committee members access

Committee members can add events from their own Google accounts instead of signing in as CES:

1. Sign in to [calendar.google.com](https://calendar.google.com) **as the CES Google account**.
2. On the left, hover over **CES Events** → click **⋮** → **Settings and sharing**.
3. Under **Share with specific people or groups**, click **Add people and groups**.
4. Add their email, set the permission to **Make changes to events**, and click **Send**.

To remove someone, click the **✕** next to their name on the same page. This is on the [handover checklist](09-committee-handover.md).

---

## Changing the calendar view

The home page calendar can show events in three ways. It's currently set to **Agenda** (decided October 2026), because the month grid is cramped on phones and most students view the site on their phones.

| View | What it looks like | Phones | Computers |
|---|---|---|---|
| `AGENDA` (current) | A scrolling list of upcoming events: date, time, title | ✅ Easy to read | OK |
| `MONTH` | A traditional month grid | ❌ Cramped | ✅ Looks like a calendar |
| `WEEK` | One week with time slots | ❌ Very cramped | OK |

The view applies to everyone. A plain Markdown site can't show one view on phones and a different one on computers. Whichever view is set, visitors can still switch between views using the tabs at the top right of the calendar itself.

### How to change it

1. On GitHub, open `index.md` and click the pencil icon ✏️ (see [01 – Editing a page](01-editing-a-page.md)).
2. Find the long line starting with `<iframe src="https://calendar.google.com/calendar/embed?`, just under the **## Calendar** heading. Press **Ctrl+F** (**Cmd+F** on a Mac) and search for `mode=` to jump to it.
3. Near the end of that line you'll see `&mode=AGENDA`. **Change only the word after `mode=`** to `MONTH` or `WEEK`, in capitals. For example, `&mode=AGENDA` becomes `&mode=MONTH`.
   - Don't change anything else on the line. The quotation marks, `&` symbols and the rest of the address must stay exactly as they are.
4. Update the word "(current)" in the grey note just above the line, so the next person knows which view is set.
5. Click **Commit changes...**, write a message like `Switch calendar to month view`, and click **Commit changes**.
6. After 1–2 minutes, check the home page on both a phone and a computer.

**Changed your mind?** Do the same steps again with the other word, or see [08 – Undoing a mistake](08-undoing-a-mistake.md).

**Calendar disappeared after the change?** Something else on the line was accidentally changed. Compare it to this, which is the exact correct line for Agenda view:

```
<iframe src="https://calendar.google.com/calendar/embed?src=d9d1f1f2576f01714405e7e2301d3a6141c72bc7d1812b0f5403b1379cc56b9e%40group.calendar.google.com&ctz=Australia%2FBrisbane&mode=AGENDA" style="border: 0" width="100%" height="600" frameborder="0" scrolling="no"></iframe>
```

You can paste that whole line back in to fix it.

---

## Setting it up again from scratch

Only needed if the CES Events calendar is ever deleted or replaced. **Time:** about 20 minutes. **You need:** the CES Google account login and a GitHub editor account.

### Part 1: Create the calendar

1. Sign in to [calendar.google.com](https://calendar.google.com) **as the CES Google account**.
2. On the left, next to **Other calendars**, click **+** → **Create new calendar**.
3. **Name:** `CES Events`. **Time zone:** `(GMT+10:00) Brisbane`. **Description:**
   > Events calendar of the Cairns Engineering Society (CES), the student engineering society at JCU Cairns. Social, industry and study events for engineering students. All times are Brisbane time (AEST). More info: https://cairns-engineering-society.github.io
4. Click **Create calendar**.

**Why a separate calendar?** Only events in *this* calendar appear on the website. The account's main calendar stays private, and subscribers see the name "CES Events" instead of an email address.

### Part 2: Make it public

1. Hover over **CES Events** → **⋮** → **Settings and sharing**.
2. Under **Access permissions for events**, tick **Make available to public**, and make sure the drop-down says **See all event details**. Confirm the warning.

### Part 3: Get the new links

On the same settings page:

| What | Where to find it |
|---|---|
| **Embed code** | **Integrate calendar** → "Embed code" (starts with `<iframe`) |
| **Google / Android subscribe link** | **Access permissions for events** → **Get shareable link** (looks like `https://calendar.google.com/calendar/u/0?cid=...`) |
| **iPhone / Outlook subscribe link** | **Integrate calendar** → "Public address in iCal format" (ends in `.ics`). Change the `https://` at the start to `webcal://`, which makes iPhones and Macs show a "Subscribe?" prompt. |

### Part 4: Update the home page

1. On GitHub, open `index.md` and click the pencil icon ✏️.
2. Under **## Calendar**, replace the whole `<iframe ...></iframe>` line with the new **embed code**. Then, in the new line:
   - change `width="800"` to `width="100%"` so it fits phone screens, and
   - add `&mode=AGENDA` to the end of the web address inside `src="..."`, just before the closing `"`.
3. Under **### Add the CES calendar to your phone**, replace the two old subscribe links with the new ones. Replace only the address inside the `( )` brackets.
4. Update the exact line in [Changing the calendar view](#changing-the-calendar-view) above and the table at the top of this guide, so they match the new calendar.
5. Commit.

### Part 5: Make a new QR code

1. Use any **free QR code generator** to make a QR code for the new **Google / Android subscribe link**.
   ⚠️ Avoid sites offering "dynamic" QR codes or free trials. Many of them **stop working after a trial period**. You want a plain **static** QR code that you download as an image.
2. Download it as a **PNG** and name it exactly `calendar-qr.png`.
3. Upload it into the `images/` folder (see [03 – Uploading a file](03-uploading-a-file.md)). Because the name is the same, it replaces the old one and the home page shows it automatically.
4. Replace the QR code on any posters or slides too.

### Check it worked

After 1–2 minutes, open the live home page. You should see the calendar and two working subscribe links. Scan the QR code with your phone to test it. Add a test event in Google Calendar, check it appears on the site within a few minutes, then delete it.

**Calendar says "Events from one or more calendars could not be shown here because you do not have permission"?** Part 2 (Make available to public) wasn't saved. Redo it.
