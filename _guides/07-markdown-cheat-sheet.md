# 07 – Markdown cheat sheet

Markdown is just text with a few symbols that turn into formatting. Everything you need for this site is on this page.

**The most common mistake:** forgetting **blank lines**. Put a blank line before and after every heading, list, table, quote and paragraph.

---

## Text

| You type | You get |
|---|---|
| `**bold**` | **bold** |
| `*italic*` | *italic* |
| `~~crossed out~~` | ~~crossed out~~ |

**New paragraph:** leave a blank line. A single line break (no blank line) gets joined onto the line above.

## Headings

```
# Page title (use only once, at the top of the page)

## Section heading

### Smaller heading
```

Always put a space after the `#` symbols.

## Links

| What | You type |
|---|---|
| A website | `[JCU](https://www.jcu.edu.au/)` |
| Another page on this site | `[Events](events.md)` |
| A section of a page | `[Calendar](index.md#calendar)` |
| A PDF in `files/` | `[Constitution](files/CES-Constitution-2025.pdf)` |
| From inside `subjects/` to a main page | `[Placement](../placement.md)` |
| An email address | `[Email CES](mailto:example@example.com)` |

The text in `[square brackets]` is what people see. The address in `(round brackets)` is where it goes. **No space** between `]` and `(`.

**Link to a section:** the part after `#` is the heading in lowercase, with spaces turned into hyphens and punctuation removed. `## What counts towards your hours` → `#what-counts-towards-your-hours`.

## Images

```
![Description of the image](images/file-name.png)
```

The description is read aloud by screen readers, so describe what's in the image.

## Lists

```
- A bullet point
- Another bullet point
  - An indented bullet (2 spaces before the -)

1. First step
2. Second step
3. Third step
```

## Quotes

```
> This is shown as a quote.
```

## Tables

```
| Column 1 | Column 2 | Column 3 |
|---|---|---|
| Row 1 | data | data |
| Row 2 | data | data |
```

- The second line (`|---|---|---|`) must be there and must have the same number of columns.
- Every row needs the same number of `|` characters.
- **No blank lines** between rows.

## Horizontal line

```
---
```

(Put a blank line above it.)

## Hidden notes for editors

```
<!-- This note is only visible to editors, never on the website. -->
```

## Dropdowns (used on the subject pages)

```
<details markdown="1">
<summary><b>Click to open</b></summary>

Hidden content goes here. **Markdown works** in here.

</details>
```

The blank line after `</summary>` and before `</details>` is required.

## Emoji

You can paste emoji straight in: 📅 ✅ ⚠️ 🎉
