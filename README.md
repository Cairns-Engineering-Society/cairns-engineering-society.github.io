# Cairns Engineering Society website – editor guide

👋 **New here? You're in the right place.** This repository holds the CES website:
**https://cairns-engineering-society.github.io**

This page only appears here on GitHub, not on the website. It's the starting point for committee members who look after the site. **No coding experience is needed.**

## How it works in 3 lines

1. Each page on the website is a `.md` text file in this repository.
2. Click a file, click the pencil icon ✏️, make your change, and click **Commit changes** (that means save).
3. The website updates itself within 1–2 minutes.

Nothing can break permanently, because every version is saved forever.

## I want to…

| I want to… | Guide |
|---|---|
| Understand how the site works (**read this first**) | [00 – How this site works](_guides/00-how-this-site-works.md) |
| Change some text on a page | [01 – Editing a page](_guides/01-editing-a-page.md) |
| Add an event | [02 – Adding an event](_guides/02-adding-an-event.md) |
| Upload a PDF or image | [03 – Uploading a file](_guides/03-uploading-a-file.md) |
| Add or update a subject | [04 – Adding a subject](_guides/04-adding-a-subject.md) |
| Add a testimonial | [05 – Adding a testimonial](_guides/05-adding-a-testimonial.md) |
| Create a whole new page | [06 – Adding a new page](_guides/06-adding-a-new-page.md) |
| Do bold text, links, lists, tables… | [07 – Markdown cheat sheet](_guides/07-markdown-cheat-sheet.md) |
| Fix something I broke | [08 – Undoing a mistake](_guides/08-undoing-a-mistake.md) |
| Hand the site over to the new committee | [09 – Committee handover](_guides/09-committee-handover.md) |
| Give someone edit access (or remove it) | [10 – Adding or removing an editor](_guides/10-adding-or-removing-an-editor.md) |
| Set up the Google Calendar (one time) | [11 – Setting up Google Calendar](_guides/11-setup-google-calendar.md) |
| Set up the Google Forms (one time) | [12 – Setting up Google Forms](_guides/12-setup-google-forms.md) |
| Switch the website on / fill in placeholders (one time) | [13 – Setting up GitHub Pages](_guides/13-setup-github-pages.md) |

## What's in this repository

| Folder / file | What it is | On the website? |
|---|---|---|
| `index.md`, `about.md`, `events.md`, … | The website pages | ✅ |
| `subjects/` | Subject pages, one per year | ✅ |
| `files/` | PDFs (constitution, minutes) | ✅ |
| `images/` | Images (calendar QR code) | ✅ |
| `_templates/` | Copy-paste blocks for events, subjects, testimonials, tips, documents and new pages | ❌ |
| `_guides/` | Step-by-step guides | ❌ |
| `_config.yml` | Site settings (rarely touched) | ❌ |
| `README.md` | This page | ❌ |

## Golden rules

1. **Everything here is public.** No phone numbers, student IDs, passwords or internal documents. Those go in the CES Google Drive.
2. **Use the templates.** They have instructions inside, and they keep everything consistent.
3. **Leave the grey `<!-- notes -->` in place.** They're hidden instructions for the next editor.
4. **Write a clear commit message**, e.g. `Add Trimester 3 BBQ`, so others can see what changed.
5. **Check the live site** 1–2 minutes after saving.
