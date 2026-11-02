# AGENTS.md --- AI Work Archive

This file defines the working rules for every AI coding agent and human
contributor in this repository.

## 1. Project purpose

Build and maintain a polished, recruiter-first personal portfolio for
Devank Gupta. The portfolio presents practical work completed with AI
tools and large language models (LLMs).

The owner is an **AI Generalist / Applied AI practitioner**. The focus
is on applying AI and LLMs to research, analysis, development,
automation and creative production---not developing or training
foundation models.

The website must communicate capability through evidence: projects, case
studies, working demonstrations and clear explanations of problems,
approaches and outcomes.

## 2. Audience priority

1.  **Primary:** Recruiters, hiring managers and potential clients.
2.  **Secondary:** Developers, technical professionals and AI
    enthusiasts.

Always make the first layer of information understandable to a
non-specialist. Put implementation details, model choices, prompts,
architecture and technical notes deeper in each case study.

## 3. Approved design direction

-   Editorial + Creative hybrid.
-   Light theme only for version 1.
-   Professional, polished, approachable and presentable.
-   Warm off-white canvas, white or near-white cards, soft corners, fine
    borders and subtle shadows.
-   Restrained muted-violet accent.
-   Strong typography hierarchy and generous whitespace.
-   Use project imagery and previews to add visual interest.
-   Motion should be subtle, purposeful and accessible.

Do not use a generic futuristic AI dashboard aesthetic. Avoid excessive
neon, glowing borders, loud gradients, clutter, gimmicky animations or
visual effects that compete with the work.

### Proposed visual tokens

Treat these as the approved starting palette; centralize them as CSS
custom properties so they can be adjusted consistently.

-   Background: `#F4F2ED`
-   Surface/card: `#FFFFFF`
-   Primary text: `#191919`
-   Secondary text: `#626262`
-   Accent: `#7156B5`
-   Border: `#E2DFD8`

Typography direction: - Plus Jakarta Sans for headings and interface
emphasis. - DM Sans for body copy and interface text. - Playfair Display
used sparingly for editorial emphasis only.

Load fonts efficiently and provide sensible system fallbacks.

### Component styling

-   Cards: approximately 12--18px corner radius.
-   Shadows: soft and low-opacity; prefer subtle borders as well.
-   Buttons: clear labels, restrained rounded treatment and visible
    focus states.
-   Hover: small elevation or image-scale change only where useful.
-   Transitions: generally 180--250ms; respect `prefers-reduced-motion`.
-   Images: consistent aspect ratios, responsive sizing and meaningful
    alt text.

## 4. Content and storytelling rules

Present work as a story or solution, not as a bare gallery of things
made.

Preferred case-study narrative: 1. Context / problem / opportunity. 2.
Objective. 3. Approach and process. 4. How AI or LLMs were applied. 5.
The owner's contribution and decisions. 6. Output, result or
demonstrated value. 7. Tools and technologies. 8. Limitations, learnings
or next steps where relevant. 9. Links to the actual work or supporting
material.

Use accurate, evidence-based language. Do not invent results, impact
metrics, users, clients, performance improvements or project completion
status. Clearly distinguish: - AI-generated output, - AI-assisted
work, - human-led work using AI as a tool, - experiments and prototypes.

Do not call the owner an AI engineer, model developer or
foundation-model expert. Suitable positioning includes: - AI
Generalist - Applied AI practitioner - AI-assisted problem solver - LLM
workflow practitioner

The positioning should emphasize practical application, judgment, tool
selection, workflow design and useful outcomes.

## 5. Approved information architecture

Version 1 uses a hybrid multi-page structure:

-   `index.html` --- homepage
-   `projects.html` --- searchable project catalogue
-   `project.html?id=<project-id>` --- individual project detail view
-   `about.html` --- background, capabilities and contact

The homepage should prioritize: 1. Hero / professional positioning. 2.
Selected work. 3. Capability areas. 4. How the owner works with AI. 5.
Tools and model ecosystem. 6. Currently building / exploring. 7. About
and contact.

The project catalogue should support: - Search by title, description and
tags. - Primary category filters. - Tool/model filters. - Year and
status filters. - Sort by newest, oldest and featured. - Grid/list view
if it remains simple and usable. - Clear links to live work, GitHub,
Drive, demos and supporting media.

Project detail pages should support mixed media and different output
types. Avoid forcing every project into an identical media layout.

## 6. Project categories

Use these nine primary categories:

1.  Development & Engineering
2.  Research & Knowledge
3.  Data Science & Analytics
4.  Graphic Design & Visual Communication
5.  Video, Animation & Motion
6.  Audio & Music
7.  Writing & Content Creation
8.  Productivity & Automation
9.  AI Experiments & Exploration

Each project has one primary category and may have multiple secondary
tags. Do not create new top-level categories without a clear
content-driven reason.

## 7. Approved technology constraints

Version 1 stack: - HTML5 - CSS3 - Vanilla JavaScript - JSON project
catalogue - Lucide icons - Git and GitHub - GitHub Pages hosting

Do not introduce React, Vue, Angular, a backend, a database,
authentication, an admin dashboard, a CMS or a build system unless the
owner explicitly approves a change.

Keep the site static and data-driven. The project catalogue should be
stored separately from presentation markup.

Use progressive enhancement where practical. The core content and
navigation should remain understandable and usable without decorative
JavaScript effects.

## 8. Suggested repository structure

``` text
ai-portfolio/
├── AGENTS.md
├── PROJECT_SPEC.md
├── index.html
├── projects.html
├── project.html
├── about.html
├── css/
│   ├── style.css
│   ├── components.css
│   └── responsive.css
├── js/
│   ├── main.js
│   ├── projects.js
│   └── filters.js
├── data/
│   ├── projects.json
│   └── tools.json
└── assets/
    ├── images/
    ├── thumbnails/
    └── icons/
```

This is a starting structure, not a mandate to create empty files
prematurely. Keep the project understandable and avoid unnecessary
fragmentation.

## 9. Project data principles

Store project information in JSON and render it through reusable
JavaScript components.

A project record should support: - Stable ID and slug. - Title and short
summary. - Primary category and tags. - Year and status. - Tools and
models used. - Output formats. - Thumbnail or preview. - Featured
flag. - External links (GitHub, Drive, live project, demo, video,
document). - Longer case-study content and optional media gallery.

Use valid JSON. Validate data and handle missing optional fields
gracefully. Do not show empty buttons or broken links.

External resources may live in Google Drive, GitHub, YouTube or other
platforms. The portfolio is an index and presentation layer; it does not
need to host every original file.

## 10. Quality requirements

Every change must preserve or improve:

-   Responsive behavior on mobile, tablet and desktop.
-   Accessible semantic HTML.
-   Keyboard navigation and visible focus.
-   Sufficient color contrast.
-   Meaningful alt text.
-   Clear link labels and safe external-link behavior.
-   Fast loading and optimized images.
-   Search/filter correctness.
-   Graceful empty states and missing-media fallbacks.
-   Descriptive page titles and metadata.
-   No horizontal overflow at common viewport widths.
-   No console errors.

Use `prefers-reduced-motion` and do not communicate status by color
alone.

## 11. Agent collaboration rules

-   Treat `PROJECT_SPEC.md` as the product and design source of truth.
-   Treat this `AGENTS.md` as the execution and contribution rulebook.
-   Read both files before making changes.
-   Do not silently change approved positioning, visual direction, page
    structure, stack or scope.
-   If a requirement is ambiguous, state the assumption or ask before
    making a consequential decision.
-   Prefer small, reviewable changes over large rewrites.
-   Do not overwrite user work or unrelated files.
-   Do not add dependencies without explaining why and obtaining
    approval.
-   Do not fabricate project content. Use clearly labelled placeholders
    until real work is inventoried.
-   Do not expose secrets, API keys, private Drive links or personal
    information.
-   Never commit credentials or private files.
-   Keep external project links configurable in data, not hard-coded
    throughout page templates.

### Parallel-agent coordination

When multiple agents work in the same repository: - Assign
non-overlapping files or clearly bounded tasks. - Do not have agents
independently edit the same files at the same time. - Have one agent
inspect/review another agent's work rather than duplicate it. -
Integrate changes through Git commits and inspect diffs before accepting
them. - The repository is the single source of truth; agents are
collaborators, not project owners.

## 12. Git and delivery rules

-   Work on a branch for substantial features when appropriate.
-   Make focused commits with descriptive messages.
-   Inspect `git status` and diffs before committing.
-   Do not force-push, delete branches or rewrite history without
    explicit approval.
-   Do not deploy or change DNS/domain settings without the owner's
    approval.
-   Before declaring a task complete, report:
    1.  What changed.
    2.  Files touched.
    3.  Tests/checks performed.
    4.  Known limitations or follow-up work.

## 13. Current scope boundaries

In scope for version 1: - Professional homepage. - Project catalogue. -
Project detail pages. - About/contact page. - Search and filtering. -
Responsive design. - External project links and media previews. -
JSON-driven content. - GitHub Pages deployment.

Not in scope unless separately approved: - User accounts. - Backend
services or database. - Admin dashboard or visual CMS. -
Analytics/tracking scripts. - Blog engine. - AI chatbot embedded in the
portfolio. - Automatic synchronization with Drive or GitHub.
