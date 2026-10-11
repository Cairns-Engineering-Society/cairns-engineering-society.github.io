# 05 – Adding a testimonial

**Time:** about 5 minutes

---

## Where testimonials come from

Students submit them using the **testimonial Google Form** (see [12 – Setting up Google Forms](12-setup-google-forms.md)). The responses are in a Google Sheet in the CES Google account.

**Before publishing, check the form response:**
- ✅ The student agreed to it being published on the website.
- ✅ You use their name **only** if they agreed to that. Otherwise write "Anonymous".
- ✅ It doesn't contain anything private (phone numbers, emails) or anything unfair about a specific named person.

You may fix obvious typos, but don't change what they meant.

## Steps

1. Open [`_templates/new-testimonial.md`](../_templates/new-testimonial.md) and copy the template block.
2. Open `testimonials.md` and click the pencil icon ✏️.
3. Paste the block **just below the grey "HOW TO ADD A TESTIMONIAL" note**, so it's above the other testimonials (newest first). Leave a blank line before and after it.
4. Replace everything in `[square brackets]`.
5. If the line `*No testimonials yet...*` is still there, delete it.
6. Click **Commit changes...**, write a message like `Add testimonial from Sam`, and click **Commit changes**.

## Check it worked

After 1–2 minutes, open the Testimonials page. The name line should be a heading and the quote should be shown as an indented quote.

## Removing a testimonial

If a student asks for theirs to be removed, do it straight away: open `testimonials.md`, delete their whole block (the `###` line and the `>` quote lines), and commit.
