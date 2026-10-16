# cloud-claude

A one-page online resume for **Thitiwut E.** (Product Engineer — web & cloud), built as a single static HTML file.

This repo is also used for learning Claude Code cloud sessions.

## What's inside

| File | Description |
| --- | --- |
| `index.html` | The resume page. All HTML and CSS live in this one file, with no build step and no JavaScript dependencies. |

The page has these sections:

- **Header**: name, role, location, and contact links (email, GitHub, LinkedIn, phone)
- **Summary**: a short profile paragraph
- **Experience**: a timeline of past roles with highlights
- **Skills**: shown as tags (TypeScript, React, Node.js, Python, SQL, Azure, Docker, CI/CD, System design)
- **Education & certifications**
- **Languages**
- **Footer**: last-updated date and a **Print / Save PDF** button

## Features

- **Responsive**: two-column layout on desktop that stacks into one column on screens narrower than 720px
- **Dark mode**: follows the system setting through `prefers-color-scheme`
- **Print-friendly**: a print stylesheet removes the background, borders, and print button so you can save a clean PDF
- **Thai-ready typography**: Google Fonts (Fraunces, IBM Plex Sans Thai, IBM Plex Mono)

## View it locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Customize

Most of the content is placeholder data (`hello@example.com`, `Company A/B/C`, `University Name`, the phone number, and the LinkedIn link). Edit `index.html` directly to put in real details.

- **Colors** are CSS variables in `:root` near the top of the `<style>` block (`--accent`, `--bg`, `--ink`, and so on), with a separate set for dark mode.
- **Experience entries** are `<article class="job">` blocks. Copy one to add another role.
- **Skills** are `<span>` elements inside `.tags`.
- Update the "Updated October 2026" date in the footer whenever you change the content.

## Deploy

The page is a static file, so any static host works. For example, with GitHub Pages: go to **Settings → Pages**, choose to deploy from the `main` branch and the root folder, and the resume will be served at `https://<user>.github.io/cloud-claude/`.
