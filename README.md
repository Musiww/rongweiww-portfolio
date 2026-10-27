# Rongwei's Portfolio 🌱

A personal corner of the internet for projects, experiments, and engineering notes.

This is **v0.1**, a deliberately simple, responsive static site built with HTML, CSS, JavaScript, and SVG. The project previews are conceptual illustrations made with code; they are not live product screenshots.

## Run locally

Open `index.html` in a browser. For a local web server (recommended), use VS Code's Live Server extension or run:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Project structure

```text
.
├── index.html                 # Page structure and content
├── styles.css                 # Design system, layout, responsiveness, animations
├── script.js                  # Mobile navigation and scroll-reveal behavior
├── favicon.svg                # Simple RW favicon
├── .github/
│   └── pull_request_template.md
├── .gitignore
└── README.md
```

## Current sections

- Hero and introduction
- About
- Projects: Mandarin Pronunciation Platform, PaySync, Timer
- Toolbox
- Résumé summary and contact section

Some links and the downloadable résumé are intentionally pending. Add only verified URLs and assets before sharing broadly.

## Working on changes

Keep `main` stable. Create a short-lived branch for one focused change, push it, open a pull request, review the diff and screenshots, and merge it when it is ready.

```bash
git switch main
git pull --ff-only
git switch -c feat/reusable-project-cards

# make changes and test locally
git status
git diff
git add .
git commit -m "refactor: extract reusable project cards"
git push -u origin feat/reusable-project-cards
```

On GitHub, open a Pull Request with `main` as the base branch and your feature branch as the compare branch. After merging, update your local `main`.

## Roadmap

- [ ] Add a verified résumé PDF and professional contact links
- [ ] Add individual project detail pages with architecture diagrams and real screenshots
- [ ] Refactor project data and previews into reusable components
- [ ] Add accessibility and responsive layout checks to CI
- [ ] Configure custom domain and deployment automation

## Attribution

Initial visual design were co-created with ChatGPT. Project descriptions reflect Rongwei's work.
