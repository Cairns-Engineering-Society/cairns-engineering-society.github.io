# Template: new subject

Use this to add a subject to one of the year pages (`subjects/year-1.md` to `subjects/year-4.md`).
Full step-by-step guide: [04 – Adding a subject](../_guides/04-adding-a-subject.md)

## Steps

1. Copy **everything** in the box below, from `<details markdown="1">` to `</details>`.
2. Open the right year page, click the pencil icon, and paste it under the right heading:
   - If **every** major takes the subject → under **Shared subjects**.
   - Otherwise → under the **first** major on its "Taken by:" line. Only write each subject once.
3. Replace everything in `[square brackets]`. Delete the square brackets too.
4. Delete the `*No subjects added yet.*` line under that heading (if it's there).
5. Click **Commit changes**.

**Don't change** the lines `<details markdown="1">`, `<summary>`, `</summary>` or `</details>`, apart from the subject code and name inside `<b>...</b>`. **Keep the blank lines** exactly as they are. They make the dropdown work.

## Copy this block

```
<details markdown="1">
<summary><b>[SUBJECT CODE] – [Subject name]</b></summary>

- **Taken by:** [e.g. Electrical core · IoT core · Mechanical minor]
- **Trimester:** [e.g. 1]
- **Official handbook page:** [JCU handbook]([paste the handbook link here])
- **Workload:** [Light / Moderate / Heavy]
- **Assessment style:** [e.g. Weekly quizzes, group project, final exam]

### What it's actually like

[2–4 sentences from students about what the subject is really like.]

### Tips from past students

- "[Tip]" ([e.g. 2025 student])
- "[Tip]" ([e.g. 2024 student])

*Last updated: [Month Year]*

</details>
```

## A finished example

This example is made up. It only shows how a finished entry looks.

```
<details markdown="1">
<summary><b>EG0000 – Example Subject</b></summary>

- **Taken by:** Electrical core · IoT core
- **Trimester:** 1
- **Official handbook page:** [JCU handbook](https://www.jcu.edu.au/)
- **Workload:** Moderate
- **Assessment style:** Weekly quizzes, group report, final exam

### What it's actually like

A broad introduction to the topic. The lectures move quickly, but the pracs are where it clicks. The group report takes more time than you'd expect.

### Tips from past students

- "Start the group report in week 3, not week 9." (2025 student)
- "Do the weekly quizzes properly. They're basically exam practice." (2024 student)

*Last updated: October 2026*

</details>
```

## Tips

- **Updating an existing subject:** open the year page, find the subject, and edit the text between its `<details markdown="1">` and `</details>` lines. Update the "Last updated" date.
- Only use student comments from the subject review form where the student agreed to be published. Use their first name or "student", never a full name unless they said yes.
- Keep it honest but fair. "The exam is hard, practise past papers" is useful. Insulting a lecturer isn't.
