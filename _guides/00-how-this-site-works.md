# 00 – How this site works (read this first)

This guide explains the big picture: what the site is, how it gets from this repository to the internet, where everything lives, and **why** it was built the way it was. You do not need to understand any code to look after this site.

---

## What this site is

The Cairns Engineering Society (CES) website is a single, free place where JCU Cairns engineering students can find:

- what CES is and how to get involved
- CES events this trimester (plus a live calendar)
- student-written descriptions of subjects ("what is this subject actually like?")
- a clear, step-by-step guide to placement
- CES documents like the constitution
- past student testimonials
- useful JCU links and "things nobody tells you"

It exists because the JCU website is hard to navigate and useful information is scattered.

**Live site:** https://cairns-engineering-society.github.io
**Repository (where the files live):** https://github.com/cairns-engineering-society/cairns-engineering-society.github.io

---

## How it works (the 30-second version)

1. Every page on the site is a plain text file ending in `.md` (a "Markdown" file) in this repository.
2. You edit a file on github.com in your web browser and click **Commit changes** (this means "save").
3. GitHub automatically turns the `.md` files into web pages. About **1–2 minutes** later the live site shows your change.

That's it. There is no server, no hosting bill, no domain to renew, and nothing to install.

> **Why "commit"?** GitHub calls saving a change a "commit". Every commit is kept forever, so any mistake can be undone (see [08 – Undoing a mistake](08-undoing-a-mistake.md)).

---

## Where everything lives

| Thing | Where | Shows on the website? |
|---|---|---|
| Website pages | `.md` files in the main folder and in `subjects/` | ✅ Yes |
| PDFs (constitution, minutes, forms) | `files/` folder | ✅ Yes, when a page links to them |
| Images (calendar QR code, photos) | `images/` folder | ✅ Yes, when a page shows them |
| Copy-paste templates | `_templates/` folder | ❌ No |
| These guides | `_guides/` folder | ❌ No |
| Instructions for editors | `README.md` | ❌ No |
| Site settings | `_config.yml` | ❌ No (it controls the site) |
| Event dates | The CES **Google Calendar** | ✅ Yes, via the calendar on the home page |
| Form responses (subject reviews, testimonials, suggestions) | **Google Forms / Sheets** in the CES Google account | ❌ No (committee copies the good ones onto the site) |
| Private committee material (passwords, internal minutes, member lists, budgets) | **CES Google Drive** – NEVER this repository | ❌ No |

**Important:** any folder or file whose name starts with `_` (an underscore) is hidden from the **website**, but this repository is **public**, so anyone who goes looking on github.com could still read it. That's fine for guides and templates. **Never put anything private in this repository.**

---

## The pages

| File | What it's for |
|---|---|
| `index.md` | Home page: welcome, quick links, latest news, calendar, subscribe links |
| `about.md` | What CES is, the committee, how to join and get involved |
| `events.md` | This trimester's events, regular events, past events |
| `placement.md` | Step-by-step placement guide |
| `things-nobody-tells-you.md` | Useful hidden knowledge, grouped by topic |
| `testimonials.md` | Past student testimonials |
| `resources.md` | Directory of hard-to-find JCU links |
| `documents.md` | Links to CES documents in `files/` |
| `subjects/index.md` | "Pick your year" page for subjects |
| `subjects/year-1.md` … `year-4.md` | Each subject in a dropdown, grouped by major |

---

## Decisions we made, and why

These were decided when the site was first built (October 2026). If you want to change one, read the reason first.

| Decision | Why |
|---|---|
| **GitHub Pages** for hosting | Free. No domain or hosting bill for the society to keep paying. |
| **Plain Markdown, default GitHub look, no custom styling** | Anyone can edit it with zero coding knowledge, and there is nothing to break or maintain. |
| **Edit directly on github.com** | Future committee members don't need to install anything or learn Git. |
| **No navigation menu**; home page has a link list and every page has "← Back to home" | A menu would need code. A list of links can't break. |
| **Google Calendar** embedded on the home page | Committee add events in the normal Google Calendar app and the site updates instantly with no GitHub edit. Students can subscribe on their phones. |
| **Subjects: one page per year, each subject in a dropdown, grouped by major** | Keeps pages short and easy to scan. Each subject is written once, with a **"Taken by:"** line (e.g. the Mechanical minor uses the Mechanical core subjects, so we don't duplicate them). |
| **Subject pages describe what subjects are *like*** and link to the official JCU handbook | We share student experience, not official content. Official details (prerequisites, credit points) change, and copying them would go out of date and raise copyright issues. |
| **Google Forms** for suggestions, subject reviews and testimonials | Students can contribute without touching GitHub. The committee reviews before anything goes live. |
| **Repository owned by the CES GitHub account; committee members use their own accounts as "collaborators"** | The site survives committee turnover. Everyone's edits are tracked under their own name. No shared password juggling. |
| **Private material in CES Google Drive, never here** | This repository is public. |
| **Templates and guides in `_` folders in the same repository** | New editors find the guides right next to the files they're editing. |

---

## Things still to be filled in

When the site was first built, some details weren't known yet. They're marked with the word **PLACEHOLDER**. To find them all: on the repository's main page, press `/` (or click the search box at the top), type `PLACEHOLDER`, and press Enter. See [13 – Setting up GitHub Pages](13-setup-github-pages.md) for what to fill in.

---

## All the guides

| Guide | Use it when you want to… |
|---|---|
| [01 – Editing a page](01-editing-a-page.md) | change any text on the site |
| [02 – Adding an event](02-adding-an-event.md) | add an event to the calendar and/or events page |
| [03 – Uploading a file](03-uploading-a-file.md) | add a PDF or image |
| [04 – Adding a subject](04-adding-a-subject.md) | add or update a subject description |
| [05 – Adding a testimonial](05-adding-a-testimonial.md) | add a student testimonial |
| [06 – Adding a new page](06-adding-a-new-page.md) | create a brand new page |
| [07 – Markdown cheat sheet](07-markdown-cheat-sheet.md) | know how to do bold, links, lists, tables… |
| [08 – Undoing a mistake](08-undoing-a-mistake.md) | fix something that broke |
| [09 – Committee handover](09-committee-handover.md) | hand the site over to a new committee |
| [10 – Adding or removing an editor](10-adding-or-removing-an-editor.md) | give someone edit access (or take it away) |
| [11 – Setting up Google Calendar](11-setup-google-calendar.md) | one-time calendar setup |
| [12 – Setting up Google Forms](12-setup-google-forms.md) | one-time forms setup |
| [13 – Setting up GitHub Pages](13-setup-github-pages.md) | one-time site setup |
