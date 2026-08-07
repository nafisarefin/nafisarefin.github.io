# nafisarefin.github.io — Hugo source

This is the **source** for [nafisarefin.github.io](https://nafisarefin.github.io/), built with
[Hugo](https://gohugo.io/) and the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme.

When this is pushed to the `main` branch of the `nafisarefin.github.io` repository, a GitHub
Actions workflow (`.github/workflows/hugo.yml`) automatically builds the site and deploys it to
GitHub Pages. **You never edit HTML by hand anymore — you edit the files below and push.**

## Where things live

| I want to change...                     | Edit this file                                   |
|-----------------------------------------|--------------------------------------------------|
| Homepage bio, photo, buttons, links     | `hugo.toml` (the `[params.profileMode]` section) |
| Social icons (CV / LinkedIn / email…)   | `hugo.toml` (the `[[params.socialIcons]]` lines) |
| Top navigation menu                     | `hugo.toml` (the `[[menu.main]]` lines)          |
| Publications list                       | `content/publications.md`                        |
| Research interests                      | `content/research.md`                            |
| Contact details                         | `content/contact.md`                             |
| Conferences                             | `content/conferences.md`                         |
| Education                               | `content/education.md`                           |
| CV page (and swap the PDF)              | `content/cv.md` (PDF is `static/cv.pdf`)         |
| Hobbies                                 | `content/hobbies.md`                             |
| A project's text / images / citation    | `content/projects/<name>.md`                     |
| Colors, spacing, custom styles          | `assets/css/extended/custom.css`                 |
| Images, PDFs, favicon                   | `static/` (referenced by path, e.g. `/dp2.png`)  |

## Adding a new project

Create one file, e.g. `content/projects/my-new-project.md`:

```markdown
---
title: "My New Project Title"
weight: 70                       # controls order in the grid (higher = lower down)
thumb: "/projects/myproj/thumb.png"
summary: "One-line description shown on the projects grid."
figures:
  - src: "/projects/myproj/fig1.png"
  - src: "/projects/myproj/fig2.png"
    style: "max-width: 400px;"
pub: 'Author A, Author B. Paper title. <em>Journal</em>, 2026.'
---

Your project description goes here — as many paragraphs as you like.
```

Put the images in `static/projects/myproj/`. The projects grid updates automatically.
(To leave a project off the grid image, just omit `thumb`; to have no side figures, omit `figures`.)

## Editing without a computer (easiest)

1. Go to the file on github.com, click the **pencil (Edit)** icon.
2. Make your change, scroll down, **Commit changes** to `main`.
3. The **Actions** tab shows the build; ~1 minute later the live site updates.

## Editing locally (optional)

Install the **extended** build of Hugo (v0.147.7 or newer), then:

```bash
hugo server        # live preview at http://localhost:1313
hugo --minify      # one-off build into ./public
```

The theme is included in `themes/PaperMod/`, so nothing else needs installing.
