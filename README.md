# Rongwei's Portfolio 🌱

A personal corner of the internet for projects, experiments, and engineering notes.

**Live site:** https://rongweiww.com

This is **v0.1**, a deliberately simple, responsive static website built with HTML, CSS, JavaScript, and SVG.

The project previews are conceptual illustrations created with code, not live product screenshots.

## Run Locally

Clone the repository and open `index.html` in a browser.

For a local development server (recommended), use VS Code's Live Server extension or run:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Project Structure

```text
.
├── index.html                   # Page structure and content
├── styles.css                   # Design system, layouts, and animations
├── script.js                    # Mobile navigation and scroll effects
├── favicon.svg                  # Custom RW favicon
├── wrangler.jsonc               # Cloudflare Workers deployment configuration
├── .github/
│   ├── workflows/
│   │   └── ci.yml               # GitHub Actions syntax checks
│   └── pull_request_template.md
├── .gitignore
└── README.md
```

## Current Sections

- **Hero & Introduction** — A brief introduction to who I am and what I enjoy building.
- **About** — My background, interests, and approach to software development.
- **Projects** — Selected engineering and development work:
  - **Mandarin Pronunciation Training Platform** — A real-time Mandarin pronunciation learning application.
  - **PaySync** — A full-stack group expense-sharing application.
  - **AWS-based Intelligent Image Processing** — A serverless image management application featuring image transformations, AI recognition, and searchable galleries.
  - **Kitten Card Game** — A Java card game focused on object-oriented design and software testing.
- **Toolbox** — Technologies and tools I work with.
- **Résumé & Contact** — Professional background and ways to connect.

Some project detail pages, demos, and downloadable assets are still in preparation.

## Development Workflow

The repository follows a lightweight Git workflow:

1. Keep `main` stable.
2. Create a short-lived feature or fix branch.
3. Make focused changes and test locally.
4. Commit and push the branch.
5. Open a pull request against `main`.
6. Review changes, CI checks, and deployment previews.
7. Merge only after verification.

Example:

```bash
git switch main
git pull --ff-only origin main
git switch -c feat/my-new-feature

# Make changes and test locally
git status
git diff
git diff --check

git add .
git commit -m "feat: describe the change"
git push -u origin feat/my-new-feature
```

After merging, update the local `main` branch before starting new work.

## CI/CD & Deployment

The portfolio is hosted on **Cloudflare** and connected to GitHub for automated deployments.

### Continuous Integration (CI)

GitHub Actions runs JavaScript syntax checks on pull requests targeting `main`.

These checks help catch syntax errors before merging, but they do not replace browser-based visual and functional testing.

### Continuous Deployment (CD)

Cloudflare Workers Builds handles deployment from the connected GitHub repository.

- **Feature branches / Pull requests:** Preview builds for reviewing changes before release.
- **`main` branch:** Production builds and deployments.
- **Custom domain:** https://rongweiww.com

Deployment settings are maintained in `wrangler.jsonc`.

Before merging changes that affect layouts or styling, verify the actual preview in a browser. A successful build does not necessarily mean the website renders correctly.

## Roadmap

- [x] Create and deploy the initial responsive portfolio
- [x] Connect a custom domain
- [x] Add GitHub Actions CI checks
- [x] Configure Cloudflare deployment previews
- [x] Expand the project showcase
- [ ] Add a verified résumé PDF and complete professional contact links
- [ ] Add individual project detail pages with architecture diagrams and real screenshots
- [ ] Refactor project data and previews into reusable components
- [ ] Add automated HTML/CSS validation and accessibility checks
- [ ] Add responsive visual regression testing
- [ ] Add a blog or engineering notes section

## Attribution

The initial visual design was developed collaboratively with ChatGPT. The website's content and project descriptions reflect Rongwei's work.

Built with curiosity, a little chaos, and lots of ww. 🌱