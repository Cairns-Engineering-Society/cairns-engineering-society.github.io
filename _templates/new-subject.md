# Template: subjects

Use this for the level pages (`subjects/level-1.md` to `subjects/level-4.md`). There are two parts:

- **Part A: add a student review** to a subject that's already listed. This is the one you'll use most. Every subject already has a dropdown with its code, name, "Taken by" line, study period and handbook link.
- **Part B: add a brand new subject** that isn't listed yet.

Full step-by-step guide: [04 – Adding a subject](../_guides/04-adding-a-subject.md)

**Don't change** the lines `<details markdown="1">`, `<summary>`, `</summary>` or `</details>`, apart from the subject code and name inside `<b>...</b>`. **Keep the blank lines** exactly as they are. They make the dropdown work.

---

## Part A: add a review to an existing subject

### Steps

1. Open the right level page (the first digit of the subject code), click the pencil icon ✏️, and find the subject. Press **Ctrl+F** (**Cmd+F** on a Mac) and type the code.
2. Inside that subject's dropdown, find the line that starts with `*No student reviews yet.`
3. **Replace that whole line** with everything in the box below.
4. Replace everything in `[square brackets]`. Delete the square brackets too.
5. Click **Commit changes**.

### Copy this block

```
- **Workload:** [Light / Moderate / Heavy]
- **Assessment style:** [e.g. Weekly quizzes, group project, final exam]

### What it's actually like

[2–4 sentences from students about what the subject is really like.]

### Tips from past students

- "[Tip]" ([e.g. 2025 student])
- "[Tip]" ([e.g. 2024 student])

*Last updated: [Month Year]. Taken this subject? [Share your experience](https://forms.gle/J5Wc61eYJdNEJ3gW7).*
```

### A finished example

This example is made up. It shows a whole subject dropdown **after** a review has been added. The first three bullet points were already there, and everything from "Workload" down is the pasted review.

```
<details markdown="1">
<summary><b>EG0000 – Example Subject</b></summary>

- **Taken by:** Electrical core · IoT core
- **When (Cairns, 2027 handbook):** Trimester 1
- **Official handbook page:** [JCU handbook](https://handbook.jcu.edu.au/)
- **Workload:** Moderate
- **Assessment style:** Weekly quizzes, group report, final exam

### What it's actually like

A broad introduction to the topic. The lectures move quickly, but the pracs are where it clicks. The group report takes more time than you'd expect.

### Tips from past students

- "Start the group report in week 3, not week 9." (2025 student)
- "Do the weekly quizzes properly. They're basically exam practice." (2024 student)

*Last updated: October 2026. Taken this subject? [Share your experience](https://forms.gle/J5Wc61eYJdNEJ3gW7).*

</details>
```

**Adding more tips later:** add another `- "[Tip]" ([year] student)` line under "Tips from past students", and update the "Last updated" date.

---

## Part B: add a new subject

Only needed if a subject isn't listed yet, e.g. a new subject, a new major, or a minor subject.

### Steps

1. Copy **everything** in the box below, from `<details markdown="1">` to `</details>`.
2. Open the right level page (the first digit of the subject code) and click the pencil icon ✏️.
3. Paste it under the heading for the group of majors that take it, e.g. `## Electrical and IoT`. Keep subjects in order of subject code, with a blank line before and after the block.
   - **No heading fits?** Add one, e.g. `## IoT and Mechanical`, with a blank line before and after.
   - Write each subject **only once**. The "Taken by:" line lists everyone who takes it.
4. Replace everything in `[square brackets]`. Delete the square brackets too.
   - **Handbook link:** search the subject in the [JCU handbook](https://handbook.jcu.edu.au/), copy the address from your browser's address bar, and paste it in. It looks like `https://handbook.jcu.edu.au/subject/2027/EG1000`.
   - **When:** the study period it runs in Cairns, shown on the handbook page (e.g. Trimester 1, Block 2).
5. Click **Commit changes**.

### Copy this block

```
<details markdown="1">
<summary><b>[SUBJECT CODE] – [Subject name]</b></summary>

- **Taken by:** [e.g. Electrical core · IoT core · Mechatronics minor (Mechanical students)]
- **When (Cairns, [year] handbook):** [e.g. Trimester 1]
- **Official handbook page:** [JCU handbook]([paste the handbook link here])

*No student reviews yet. Taken this subject? [Share your experience](https://forms.gle/J5Wc61eYJdNEJ3gW7).*

</details>
```

---

## Tips

- Only use student comments from the subject review form where the student agreed to be published. Credit them the way they chose on the form (first name, year only, or not at all). Never use a full name.
- Combine several responses into one fair summary, and pick the most useful tips.
- Keep it honest but fair. "The exam is hard, practise past papers" is useful. Insulting a lecturer isn't.
