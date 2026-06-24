# Editing and Deployment Instructions

This website is intentionally simple. There is no build system, no database, and no special app to run. Each page is a plain `.html` file.

## Change Text

1. Open the page you want to edit, such as `about.html` or `resume.html`.
2. Look for the visible sentence you want to change.
3. Replace only the text between the HTML tags.

Example:

```html
<p>
  Replace this sentence with the new sentence.
</p>
```

Do not delete the opening tag, such as `<p>`, or the closing tag, such as `</p>`.

## Change Navigation Labels

The navigation appears near the top of each `.html` file inside this block:

```html
<nav class="site-nav" id="site-nav" aria-label="Primary navigation">
```

If you rename a page in the navigation, update the same label on every page so the menu stays consistent.

## Add a Case Study

1. Open `case-studies.html`.
2. Find this comment:

```html
<!-- To add a case study: copy one full article.case-study block, paste it below, update the id, number, title, and text. -->
```

3. Copy one full block that starts with:

```html
<article class="case-study" id="example-id">
```

and ends with:

```html
</article>
```

4. Paste it below the existing case studies.
5. Change the `id`, case study number, title, summary, challenge, approach, and potential impact.

Use short, concrete language. Do not include confidential employer, client, member, or patient details.

## Add a Project

1. Open `projects.html`.
2. Copy one full `<article class="card project-card">` block.
3. Paste it inside the `<div class="card-grid two">` section.
4. Update the label, title, description, and link.

## Add a Writing Item

1. Open `writing.html`.
2. Copy one full `<article class="writing-item">` block.
3. Paste it below the existing writing items.
4. Update the label, title, and summary.

## Update Contact Information

Open `contact.html` and update:

- the email link
- the LinkedIn link
- the GitHub link
- the best-fit conversation areas

For the email link, update both the visible email and the `mailto:` value.

## Deploy Changes

This site is published through GitHub Pages.

After changing files:

1. Save the files.
2. Commit the changes in Git.
3. Push to the `main` branch of `clarejordan/clarejordan.github.io`.
4. Wait a few minutes.
5. Visit `https://clarejordan.github.io/`.

GitHub Pages updates automatically after the push.

## Custom Domain Later

When a custom domain is purchased, add it in the GitHub Pages settings for the repository. The likely domain recommendation remains `clareljordan.com`, if available.
