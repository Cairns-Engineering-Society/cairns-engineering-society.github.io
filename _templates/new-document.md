# Template: new document

Use this to list a document (PDF) on the **CES documents** page (`documents.md`).
Full step-by-step guide: [03 – Uploading a file](../_guides/03-uploading-a-file.md)

## Before you start

- Only upload documents that are fine for **anyone on the internet** to read. Internal documents go in the CES Google Drive.
- Upload the PDF into the `files/` folder **first**. Give it a name with **no spaces**, using hyphens instead, e.g. `CES-Constitution.pdf`.

## Steps

1. Copy the **one line** in the box below.
2. Open `documents.md`, click the pencil icon, and paste it on a new line **directly under the last row** of the right table. If the section says `*No ... uploaded yet.*`, replace that line with the table header from the example below, then your row.
3. Replace everything in `[square brackets]`. The file name must match the uploaded file **exactly**, including capital letters and `.pdf`.
4. Click **Commit changes**, then open the live site and click the link to check it works.

## Copy this line

```
| [Document name](files/[exact-file-name.pdf]) | [What it is, one short sentence] | [Date or year] |
```

## A finished example

A table with its header row and one document:

```
| Document | What it is | Last updated |
|---|---|---|
| [AGM Minutes 2026](files/CES-AGM-Minutes-2026.pdf) | Minutes from the 2026 Annual General Meeting | March 2026 |
```

## Replacing a document with a new version

Upload the new PDF with the **same file name**. GitHub will replace the old one, and the existing link keeps working. Update the "Last updated" column.
