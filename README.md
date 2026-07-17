# Dean Hattenhauer - Resume Generator

A JSON-schema-driven resume system that generates both an ATS-safe PDF and a styled web version from a single source of truth. Update `resume.json` once, and the build process propagates changes across every rendered output.

## What This Is

- **Single source of truth**: `resume.json` holds all resume content (experience, skills, projects, certifications).
- **Dual output**: Generates an ATS-safe PDF (Paper theme) for job applications and a styled web version (Elegant theme) for the live portfolio site.
- **Live site**: Deployed at [deanhattenhauer.dev](https://deanhattenhauer.dev)

## Tech Stack

- Node.js / npm
- [resume-cli](https://www.npmjs.com/package/resume-cli) — resume rendering engine
- JSON Resume schema
- Puppeteer (via Chrome) for PDF export
- GitHub Pages for hosting

## Setup

1. Clone the repo
2. Install dependencies:
   \`\`\`bash
   npm install
   \`\`\`
3. Confirm `resume.json` is present in the project root

## Quick Start

Preview the resume locally:

\`\`\`bash
npm run preview:elegant
\`\`\`

Build both outputs (PDF + web HTML):

\`\`\`bash
npm run build:all
\`\`\`

Serve the built web version locally:

\`\`\`bash
npm run serve:web
\`\`\`
Then visit http://localhost:4000

## Updating Content

For the full step-by-step update and deployment workflow, see [`update.md`](./update.md).

## Themes

- **Paper** — ATS-safe, used for the exported PDF resume
- **Elegant** — styled web version with icons and layout, used for the live site
- Flat and Spartan themes also available as dev dependencies, not currently used in build scripts

## Live Site

[deanhattenhauer.dev](https://deanhattenhauer.dev)
