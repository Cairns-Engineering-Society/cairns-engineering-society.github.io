# 04 – Adding or updating a subject

Subjects are on the year pages: `subjects/year-1.md` to `subjects/year-4.md`. On the website, each subject is a **dropdown**: students click the name to open it.

**Time:** about 10 minutes per subject

---

## Where the content comes from

The subject descriptions are written from **student experience**. They usually come from the **subject review Google Form** (see [12 – Setting up Google Forms](12-setup-google-forms.md)). The responses are in a Google Sheet in the CES Google account.

**Only use** responses where the student agreed to be published. Combine several responses into one fair summary, and pick the most useful tips.

## Where the subject goes

Each year page has four headings:

| Heading | Put a subject here if… |
|---|---|
| **Shared subjects (all majors)** | **every** major takes it |
| **Electrical** | it's not shared, and Electrical is the first major on its "Taken by:" line |
| **IoT** | it's not shared, and IoT is the first major on its "Taken by:" line |
| **Mechanical (core and Mechanical minor)** | it's a Mechanical subject. The Mechanical minor uses the Mechanical core subjects, so they're written once here. |

**Write each subject only once.** The "Taken by:" line tells students who takes it, e.g. `Mechanical core · Mechanical minor (Electrical & IoT students)`.

## Steps: add a new subject

1. Open [`_templates/new-subject.md`](../_templates/new-subject.md) and copy the **whole** block, from `<details markdown="1">` to `</details>`.
2. Open the right year page (`subjects` folder → `year-1.md` etc.) and click the pencil icon ✏️.
3. Paste the block under the right heading. Leave a **blank line** before and after it. If there are other subjects there, keep them in order of subject code.
4. If the heading has a line saying `*No subjects added yet.*`, delete that line.
5. Replace everything in `[square brackets]`:
   - **Subject code and name** go inside `<b>...</b>` on the `<summary>` line.
   - **Handbook link:** find the subject in the JCU handbook, copy the address from your browser's address bar, and paste it in place of `[paste the handbook link here]`. It should end up like `[JCU handbook](https://...)`.
   - Set the **Last updated** date.
6. Click the **Preview** tab to check it. (The preview on GitHub may look slightly different from the live site, which is normal.)
7. Click **Commit changes...**, write a message like `Add EG1000 to year 1`, and click **Commit changes**.

## Steps: update an existing subject

1. Open the year page and click the pencil icon ✏️.
2. Find the subject. Press **Ctrl+F** (Windows) or **Cmd+F** (Mac) and type the subject code.
3. Edit the text **between** its `<details markdown="1">` and `</details>` lines, e.g. add a new tip.
4. Update **Last updated**.
5. Commit.

## Check it worked

After 1–2 minutes, open the year page on the live site, click the subject name and check it opens properly.

**Something looks wrong?**

| Problem | Fix |
|---|---|
| The subject shows with `**` stars or `###` instead of bold text and headings | There's a **blank line missing** straight after the `</summary>` line, or straight before `</details>`. Add it. |
| Everything below the subject is stuck inside its dropdown | The `</details>` line is missing or misspelled. |
| The dropdown doesn't appear at all | Check the first line is exactly `<details markdown="1">`. |

## Adding a new major or minor later

If a new major starts (or you want a separate heading for a minor), add a heading to each year page, e.g. `## Civil`, with a blank line before and after, and a `*No subjects added yet.*` line under it. Then update the table at the top of this guide and [`subjects/index.md`](../subjects/index.md).
