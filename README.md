# Sherry Hu — Personal Website

A Hugo website using the real PaperMod theme, with a custom visual homepage and project portfolio. Includes five projects, background, education, interests, skills, learning notes, a Now page, search, project filters, and light/dark mode.

## Publish on GitHub Pages

1. Create a **new public repository** named `sherryhuproducts.github.io` under `SherryHuProducts`. Keep your existing profile repository `SherryHuProducts` separate.
2. Unzip the supplied source package. Open the project folder in VS Code.
3. Initialize the folder as a Git repository and push it to the new repository's `main` branch using VS Code Source Control / Publish Branch or your normal Git workflow. Include `.github/workflows/pages.yaml`; Finder hides `.github` by default, but VS Code displays it.
4. In GitHub, open **Settings → Pages → Source → GitHub Actions**.
5. Run the **Build and deploy personal website** workflow from the Actions tab if the first push ran before Pages was configured.
6. After a successful workflow, visit `https://sherryhuproducts.github.io`.

The workflow installs pinned Hugo v0.167.0 and builds from the vendored theme. No Ruby, Jekyll, Node installation, purchased domain, or manual local build is needed for GitHub publication.

## Local preview (optional)

Install Hugo v0.167.0, then run:

```sh
hugo server
```

Open the address printed by Hugo, usually `http://localhost:1313`.

## Edit content

| Content | File / folder |
|---|---|
| Bio, work experience, education, skills, interests | `content/about.md` |
| Current learning | `content/now.md` |
| Project case studies | `content/projects/` |
| Learning notes | `content/notes/` |
| Homepage introduction and layout | `layouts/home.html` |
| Colors, typography, responsive layout | `assets/css/extended/sherry.css` |
| Title, navigation, default URL | `hugo.yaml` |

To add a learning note, create a `.md` file under `content/notes/` with a title, date, and tags in its front matter. Markdown content becomes a page after the next push. RSS and search indexes rebuild automatically. The initial three notes are marked as working drafts in their content; review or revise them before presenting them as final writing.

## First content review

- Confirm your preferred public name, city wording, work dates, and role descriptions.
- Review the three initial working notes, prepared from your public project descriptions.
- Add a chosen profile photo, LinkedIn URL, contact method, or public resume only when ready.
- Keep project status explicit: synthetic case studies, simulated payment provider, and features still planned.

## Template

Upstream theme: https://github.com/adityatelange/hugo-PaperMod
See `TEMPLATE-ATTRIBUTION.md` and `themes/PaperMod/LICENSE`.
