# 04 – Adding a subject review (or a new subject)

Subjects are on the **level pages**: `subjects/level-1.md` to `subjects/level-4.md`. A subject's level is the **first digit of its code** (EG**2**008 → level 2). On the website, each subject is a **dropdown**: students click the name to open it.

Every subject in the 2027 handbook for the Cairns majors and the Mechatronics minor is **already listed**, with its code, name, who takes it, when it runs in Cairns, and a handbook link. Most of the time you'll just be **adding a student review** to one.

**Time:** about 10 minutes per subject

---

## Where the reviews come from

The subject descriptions are written from **student experience**. They usually come from the **subject review Google Form** (see [12 – Setting up Google Forms](12-setup-google-forms.md)). The responses are in a Google Sheet in the CES Google account.

**Only use** responses where the student agreed to be published, and credit them the way they chose. Combine several responses into one fair summary, and pick the most useful tips.

## How the level pages are organised

Each level page groups subjects by **who takes them**. Only the groups that have subjects at that level appear.

| Group heading | Means |
|---|---|
| **Core (all majors)** | Every major takes it |
| **Electrical, IoT and Mechanical** / **Electrical and IoT** / **Electrical and Mechanical** | Shared by those majors |
| **Electrical only** / **IoT only** | Just that major |
| **Mechanical** / **Mechanical and Maritime** | Mechanical core (Level 2 is shared with Maritime) |
| **Maritime** | Maritime-only subjects and the extra conditions (Cairns for 2 years, then Tasmania) |
| **Mechatronics minor** | Subjects that are only in the Mechatronics minor |

**Write each subject only once.** The **"Taken by:"** line tells students everyone who takes it, e.g. `Mechanical core · Maritime core · Mechatronics minor (Electrical & IoT students)`.

## Steps: add a review to an existing subject

1. Open [`_templates/new-subject.md`](../_templates/new-subject.md) and copy the **Part A** block.
2. Open the right level page (`subjects` folder → `level-1.md` etc.) and click the pencil icon ✏️.
3. Find the subject. Press **Ctrl+F** (Windows) or **Cmd+F** (Mac) and type the subject code.
4. Inside its dropdown, **replace the line** that starts with `*No student reviews yet.` with the block you copied.
5. Replace everything in `[square brackets]` and set the **Last updated** date.
6. Click the **Preview** tab to check it. (The preview on GitHub may look slightly different from the live site, which is normal.)
7. Click **Commit changes...**, write a message like `Add review for EG1000`, and click **Commit changes**.

**Adding more tips to a subject that already has a review:** add another tip line under "Tips from past students" and update the **Last updated** date.

## Steps: add a new subject

Only needed for subjects that aren't listed yet, e.g. new subjects, a new major, or other minors.

1. Copy the **Part B** block from [`_templates/new-subject.md`](../_templates/new-subject.md).
2. Open the right level page and paste it under the heading for the group that takes it, in order of subject code. Leave a blank line before and after.
3. Fill in the code, name, "Taken by", "When" and handbook link. The template explains where to find each one.
4. Commit.

## Check it worked

After 1–2 minutes, open the level page on the live site, click the subject name and check it opens properly.

**Something looks wrong?**

| Problem | Fix |
|---|---|
| The subject shows with `**` stars or `###` instead of bold text and headings | There's a **blank line missing** straight after the `</summary>` line, or straight before `</details>`. Add it. |
| Everything below the subject is stuck inside its dropdown | The `</details>` line is missing or misspelled. |
| The dropdown doesn't appear at all | Check the first line is exactly `<details markdown="1">`. |

---

## Each new year: updating for the new handbook

JCU publishes a new handbook each year, and subjects or study periods sometimes change. Once a year (e.g. at [handover](09-committee-handover.md)):

1. Check each major's handbook page (linked from [`degree.md`](../degree.md)) for added or removed subjects.
2. Add new subjects (Part B), and delete the dropdowns of subjects that no longer exist. Delete from `<details markdown="1">` to `</details>`.
3. Update the **When** lines if study periods changed, and change `2027` in the handbook links and "When (Cairns, 2027 handbook)" lines to the new year. Press **Ctrl+F** (**Cmd+F** on a Mac) and search for `2027` to find each one.

## Adding a new major or minor later

Add a heading for it on each level page where it has subjects (e.g. `## Civil`), with a blank line before and after. Then add its subjects using Part B, add it to the "Taken by" lines of shared subjects, and update the table above and [`subjects/index.md`](../subjects/index.md).
