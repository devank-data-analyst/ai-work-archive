# PROJECT_SPEC.md --- AI Work Archive / Personal Portfolio

**Owner:** Devank Gupta\
**Version:** 1.0\
**Status:** Approved direction; ready for visual prototype\
**Working title:** DEVANK. --- AI Work Archive

------------------------------------------------------------------------

## 1. Executive summary

Build a polished, recruiter-first personal portfolio that organizes and
presents work completed using artificial intelligence and large language
models (LLMs).

The website is more than a gallery. It is a curated archive and
professional presentation layer for a diverse body of work: web
applications, research documents, images, collages, posters, explanatory
diagrams, videos, data analysis, Telegram bots, writing, automation and
experiments.

The owner will discover and add work gradually during the project. The
site must therefore be easy to maintain and designed to grow as the
archive becomes more complete.

The portfolio should help a visitor quickly understand: - What the owner
can do with AI and LLMs. - How the owner applies AI across different
domains. - What practical work and outputs demonstrate those
capabilities. - How to inspect the underlying work, code or supporting
documents.

## 2. Professional positioning

### Core identity

**AI Generalist --- Applied AI, LLM Workflows and Creative Technology**

The owner's strength is the practical application of AI and LLMs, not
the development or training of foundation models.

The portfolio should communicate: - Familiarity with multiple AI tools
and LLMs. - Ability to select and apply tools to different tasks. -
Research, analysis and synthesis. - AI-assisted development and
technical problem-solving. - Creative production across image, video,
audio and writing. - Workflow design, automation and productivity. -
Ability to evaluate outputs, iterate and combine AI with existing tools.

Avoid unsupported claims such as "AI expert", "AI engineer", "model
developer" or "expert in every AI tool".

### Proposed headline

**Making AI useful beyond the conversation.**

Supporting statement:

"I explore and apply AI and large language models across research,
development, data analysis and creative production --- turning ideas
into practical solutions and meaningful work."

This copy is a starting point and may be refined during prototype
review.

## 3. Audience and communication priorities

### Primary audience

-   Recruiters
-   Hiring managers
-   Potential employers
-   Clients and collaborators

### Secondary audience

-   Developers
-   Technical professionals
-   AI enthusiasts and power users

### Communication rule

The first layer must be approachable to a non-specialist. Lead with the
problem, approach and outcome. Put technical depth in the case study.

A recruiter should be able to understand the owner's capabilities and
inspect credible evidence within approximately 30 seconds.

A technical visitor should be able to go deeper into tools, models,
prompts, workflows, architecture, code and limitations.

## 4. Product intent and content philosophy

The portfolio should tell stories about solving problems and producing
useful outcomes---not simply say "look what I made".

Preferred framing:

-   "Reducing repetitive work through conversational automation."
-   "Turning a complex dataset into actionable insights."
-   "Exploring visual storytelling through AI-assisted animation."

Avoid generic framing:

-   "Here is my bot."
-   "Some images I generated."
-   "Tools I know."

Every project should explain, where applicable: 1. Context or problem.
2. Objective. 3. Approach and process. 4. How AI/LLMs were used. 5. The
owner's contribution and decisions. 6. Output, result or demonstrated
value. 7. Tools and technologies. 8. Limitations, learning or next
steps. 9. Links to the real work.

Never invent outcomes, impact metrics, clients, users or completion
status. Distinguish AI-generated, AI-assisted, human-led and
experimental work accurately.

## 5. Brand and visual direction

### Chosen direction

**Editorial + Creative hybrid, professional and recruiter-first.**

The visual experience should feel like a polished creative-technology
portfolio or an editorial publication---not a futuristic AI dashboard,
developer terminal or generic template gallery.

### Design qualities

-   Approachable and professional.
-   Clean, composed and confident.
-   Warm and human rather than sterile.
-   Strong typographic hierarchy.
-   Generous whitespace.
-   Softly rounded cards.
-   Subtle shadows and fine borders.
-   Carefully selected media previews.
-   restrained use of color and motion.

### Explicitly avoid

-   Neon cyberpunk styling.
-   Excessive glowing borders.
-   Loud gradients and decorative effects.
-   Dense dashboard layouts.
-   Excessive animation.
-   Overly playful or gimmicky interactions.
-   Project cards that are only screenshots with no context.

### Theme

**Light theme only for version 1.** Do not implement a dark/light toggle
in the initial release.

### Proposed color palette

  Token            Value       Usage
  ---------------- ----------- -------------------------------------
  Background       `#F4F2ED`   Main page canvas
  Surface          `#FFFFFF`   Cards and panels
  Primary text     `#191919`   Headlines and body
  Secondary text   `#626262`   Supporting copy
  Accent           `#7156B5`   Links, small highlights and actions
  Border           `#E2DFD8`   Card and section boundaries

Use CSS custom properties for all design tokens. Check contrast in
actual implementation; adjust if needed for accessibility.

### Typography

Proposed font combination: - **Plus Jakarta Sans:** headings and
interface emphasis. - **DM Sans:** body text, labels and navigation. -
**Playfair Display:** selective editorial emphasis only.

The typography should have character without reducing readability. Use
appropriate weights and line lengths. Provide system fallbacks and load
only the font weights actually used.

### Components and interaction

  Element       Direction
  ------------- --------------------------------------
  Cards         12--18px corner radius
  Shadows       Soft, subtle and low-opacity
  Borders       Fine neutral borders
  Buttons       Clear, restrained rounded buttons
  Hover         Small elevation or subtle image zoom
  Transitions   Around 180--250ms
  Spacing       Generous and consistent
  Images        Responsive, consistent aspect ratios

Respect `prefers-reduced-motion`. Keep focus states visible and keyboard
navigation usable.

## 6. Information architecture

Use a hybrid multi-page website.

### Page 1 --- Homepage (`index.html`)

Purpose: communicate identity, capability and strongest evidence
quickly.

Recommended section order:

1.  **Navigation**
    -   Personal wordmark: `DEVANK.`
    -   Links to Work, About and Contact.
    -   Keep navigation compact and clear.
2.  **Hero / Professional positioning**
    -   Name and applied-AI positioning.
    -   Headline: "Making AI useful beyond the conversation."
    -   Short supporting statement.
    -   Primary CTA: Explore selected work.
    -   Secondary CTA: Get in touch / About.
3.  **Selected work**
    -   Three to four featured projects once real projects are selected.
    -   Cards lead with problem/solution-oriented titles.
    -   Use real project previews when available.
    -   Clearly mark sample content as placeholder during development.
4.  **What I do / Capability areas**
    -   Applied AI and LLM workflows.
    -   Research and analysis.
    -   AI-assisted development and automation.
    -   Creative production and visual communication.
    -   Data analysis and problem-solving.
5.  **How I work**
    -   Understand the task or problem.
    -   Select suitable models and tools.
    -   Design prompts and workflows.
    -   Validate, iterate and combine outputs with conventional tools.
    -   Deliver and document a usable result.
6.  **Tools and model ecosystem**
    -   Display tools the owner has actually used.
    -   Do not imply proficiency from a name-only list.
    -   Optionally distinguish regular use, practical experience and
        exploration.
7.  **Currently building / exploring**
    -   Ongoing projects and learning.
    -   Show status honestly.
8.  **About and contact**
    -   Concise personal background.
    -   Relevant links and contact method.
9.  **Footer**
    -   GitHub, LinkedIn, email and other confirmed public profiles.

### Page 2 --- Project catalogue (`projects.html`)

Purpose: provide a searchable, organized archive of the owner's work.

Required functionality: - Search title, summary, description and tags. -
Filter by primary category. - Filter by tools/models where useful. -
Filter by year. - Filter by status. - Sort newest, oldest and
featured. - Grid/list view if it can be implemented cleanly. - Clear
empty state and reset-filters action.

Project card content: - Thumbnail or media preview. - Title. -
Outcome-oriented short summary. - Primary category. - Year and status. -
Relevant tools or tags. - Link to the project detail page.

Keep the interface simple. Do not let filters overwhelm the project
cards.

### Page 3 --- Project detail (`project.html?id=<project-id>`)

Purpose: tell the full project story and link to evidence.

Use a reusable page template driven by project data. Support: - Overview
and context. - Problem/objective. - Approach and process. - AI's role
and owner's contribution. - Output/result. - Tools and models. -
Technical breakdown where relevant. - Image gallery. - Video embed. -
PDF/document link. - GitHub repository. - Live demo/application. - Drive
or external source link. - Learnings and limitations.

The page should gracefully omit sections that do not apply. Do not show
empty link buttons or broken embeds.

### Page 4 --- About (`about.html`)

Purpose: provide professional context.

Possible content: - Applied-AI positioning. - Background and interests
relevant to work. - Capability overview. - How the owner approaches
AI-assisted work. - Contact and professional links.

Keep the About page concise and evidence-oriented.

## 7. Main project categories

Organize work by the type of output or capability---not by the AI tool
used.

1.  **Development & Engineering**
    -   Web applications, websites, Telegram bots, scripts, APIs,
        prototypes, software experiments.
2.  **Research & Knowledge**
    -   Research documents, reports, comparative studies,
        investigations, literature reviews, technical documentation,
        knowledge summaries.
3.  **Data Science & Analytics**
    -   Data cleaning, EDA, statistical analysis, Python notebooks,
        dashboards, visualizations, datasets, analytical reports.
4.  **Graphic Design & Visual Communication**
    -   Posters, photo collages, infographics, explanatory diagrams,
        presentations, illustrations, logos, social graphics.
5.  **Video, Animation & Motion**
    -   AI-generated videos, animation, music videos, promotional
        videos, motion graphics, storyboards, video editing.
6.  **Audio & Music**
    -   Music generation, lyrics, songwriting, voice generation, sound
        design, audio editing, voiceovers.
7.  **Writing & Content Creation**
    -   Articles, blogs, scripts, creative writing, poetry,
        documentation, copywriting, prompts, content strategy.
8.  **Productivity & Automation**
    -   Automated workflows, AI agents, integrations, data processing,
        productivity systems, repeatable processes.
9.  **AI Experiments & Exploration**
    -   Prompt experiments, LLM comparisons, model testing, reasoning
        experiments, multimodal exploration, proof-of-concepts.

Each project has one primary category and may have multiple secondary
tags. Add subcategories only when the real archive demonstrates a need.

## 8. Project metadata and data model

Keep content separate from presentation using JSON.

### Proposed project record

``` json
{
  "id": "project-001",
  "slug": "project-name",
  "title": "Project Name",
  "category": "development-engineering",
  "tags": ["LLM", "Automation"],
  "year": 2026,
  "status": "completed",
  "contribution_type": "ai-assisted",
  "tools": ["ChatGPT", "Claude"],
  "formats": ["Web app", "PDF"],
  "summary": "A concise, outcome-oriented summary.",
  "description": "A fuller project description.",
  "thumbnail": "assets/thumbnails/project-name.webp",
  "featured": true,
  "links": {
    "github": "",
    "drive": "",
    "live": "",
    "demo": "",
    "video": ""
  }
}
```

The final schema may be extended to support: - Problem/context. -
Objective. - Approach. - AI's role. - Owner's contribution. -
Outcomes. - Technical details. - Limitations and learnings. - Media
gallery. - Additional external resources.

### Metadata conventions

-   `status`: completed, ongoing, experimental, archived or abandoned.
-   `contribution_type`: ai-generated, ai-assisted, human-led-with-ai,
    hybrid.
-   `year`: year of the work or meaningful project milestone.
-   `category`: one approved primary category.
-   `tools`: only tools actually used for that project.
-   `links`: optional; only show links that exist and are accessible.

The JSON catalogue should be easy to edit manually. Validate it and
handle missing fields safely.

## 9. Technology stack

### Approved version 1 stack

  -----------------------------------------------------------------------
  Layer                   Technology              Purpose
  ----------------------- ----------------------- -----------------------
  Structure               HTML5                   Semantic page structure

  Styling                 CSS3                    Layout, design tokens,
                                                  responsive UI

  Interactions            Vanilla JavaScript      Search, filters,
                                                  navigation and
                                                  rendering

  Content                 JSON                    Project and tool
                                                  catalogue

  Icons                   Lucide                  Consistent interface
                                                  icons

  Fonts                   Google Fonts or locally Typography
                          hosted alternatives     

  Version control         Git + GitHub            Source and
                                                  collaboration

  Hosting                 GitHub Pages            Static website
                                                  deployment
  -----------------------------------------------------------------------

### Architecture principles

-   Static website; no server required.
-   No database in version 1.
-   JSON is the content source of truth.
-   Reusable components and templates.
-   Keep markup, styling, behavior and content separated.
-   Avoid unnecessary dependencies.
-   Build for maintainability and easy future migration.

Do not introduce React, a CSS framework, backend, database,
authentication or CMS without an explicit decision.

## 10. Repository structure

Proposed starting structure:

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

The structure may be adjusted if a simpler arrangement is more
appropriate. Avoid creating empty files or abstractions without a
current need.

## 11. Media and external-link strategy

The website is a presentation and indexing layer. It does not need to
store every original project file.

  Content                Preferred location
  ---------------------- ----------------------------------------
  Website source         GitHub repository
  Code projects          GitHub repositories
  Project metadata       JSON in portfolio repository
  Research documents     Google Drive or public document links
  Large original media   Google Drive or suitable media hosting
  Website thumbnails     Optimized local assets
  Video demonstrations   YouTube or supported embeds
  Live applications      Their deployed URLs

Important: - Verify sharing permissions before publishing Drive links. -
Do not publish private documents or personal data. - Do not commit API
keys, tokens or credentials. - Use local optimized thumbnails rather
than relying on fragile external image URLs. - For external links, use
descriptive labels and safe `target="_blank"` handling with
`rel="noopener noreferrer"` where appropriate. - Test every public link
before deployment. - Use a fallback when an embed is unavailable.

## 12. Hosting, domain and available resources

### Hosting

Use GitHub Pages for the first release. It is suitable for a static
HTML/CSS/JavaScript portfolio.

### GitHub Education

The owner has access to GitHub Education. Use relevant benefits where
they genuinely help, but do not add services just because they are
included.

### Domain

The owner has access to one-year domain offers through Namecheap and
Name.com.

A previously used domain, `devank.site`, may be relevant. Confirm
current ownership and control before making domain changes or buying
another domain.

Potential domain direction: - Prefer a personal identity that can
support future work beyond AI. - Compare first-year cost, renewal price,
privacy and DNS management. - Do not purchase or configure a domain
without the owner's approval.

### Deployment plan

1.  Create and verify the GitHub repository.
2.  Build and test locally.
3.  Push the approved version.
4.  Enable GitHub Pages.
5.  Verify the published site.
6.  Connect a custom domain only after approval.
7.  Verify HTTPS, DNS and redirects.

## 13. AI-assisted development workflow

The owner intends to use: - **Google Antigravity:** visual exploration,
UI prototyping, browser inspection and parallel agent tasks. - **OpenAI
Codex:** implementation, refactoring, debugging, testing and code
review. - **ChatGPT:** product direction, planning, writing, critique
and coordination.

These tools are collaborators. The Git repository is the single source
of truth.

Recommended division: - Antigravity: explore layouts, propose visual
options, prototype UI and inspect rendered results. - Codex: implement
approved designs, maintain code quality, debug and review. - ChatGPT +
owner: define requirements, approve design decisions, prioritize work
and review deliverables.

All agents must read `AGENTS.md` and this specification before working.
Avoid simultaneous edits to the same files. Use Git diffs and commits to
integrate work.

## 14. Non-functional requirements

-   Responsive on desktop, tablet and mobile.
-   Semantic HTML and accessible controls.
-   Keyboard navigation and visible focus indicators.
-   Sufficient color contrast.
-   Meaningful image alt text.
-   No horizontal overflow.
-   Optimized images and reasonable page weight.
-   Fast initial rendering.
-   Clear page titles and meta descriptions.
-   Search and filters work correctly.
-   Graceful missing-content and empty states.
-   No broken links or console errors.
-   Reduced-motion preference respected.
-   No unnecessary tracking or third-party scripts.

## 15. Version 1 scope

### Included

-   Light-theme professional homepage.
-   Searchable project catalogue.
-   Individual project detail pages.
-   About/contact page.
-   Nine project categories.
-   Search and filtering.
-   Project metadata in JSON.
-   External links and media previews.
-   Responsive design.
-   GitHub Pages deployment.

### Not included initially

-   Dark theme or theme toggle.
-   User accounts.
-   Backend or database.
-   Admin dashboard.
-   Visual CMS.
-   Automatic Drive/GitHub synchronization.
-   Embedded AI chatbot.
-   Blog engine.
-   Complex analytics.

These may be reconsidered after the portfolio is populated and real
needs emerge.

## 16. Development roadmap

### Phase 1 --- Foundation

-   Create repository and project files.
-   Add `AGENTS.md` and `PROJECT_SPEC.md`.
-   Establish CSS tokens, typography and responsive foundations.
-   Build shared navigation, buttons, cards and footer.

### Phase 2 --- Visual prototype

-   Create homepage using clearly marked sample content.
-   Explore and review layout alternatives.
-   Test desktop and mobile layouts.
-   Finalize visual details before building all pages.

### Phase 3 --- Project catalogue

-   Define and validate JSON schema.
-   Render project cards.
-   Implement search, category/tool/year/status filters.
-   Add sorting and empty states.

### Phase 4 --- Project details

-   Implement dynamic detail pages.
-   Support mixed media and external links.
-   Add recruiter-friendly story structure and optional technical
    breakdown.

### Phase 5 --- Content inventory and population

-   Discover work across local folders, Drive, GitHub and AI platforms.
-   Record each item in an inventory.
-   Classify it into a primary category and tags.
-   Verify source links and permissions.
-   Add accurate descriptions and previews.
-   Mark ongoing, experimental or incomplete work honestly.

### Phase 6 --- Quality assurance and deployment

-   Test across viewport sizes.
-   Check accessibility, links, performance and console.
-   Review all claims and project descriptions.
-   Deploy through GitHub Pages.
-   Connect the approved domain if desired.

## 17. Acceptance criteria

Version 1 is ready to publish when:

1.  A first-time visitor can understand the owner's applied-AI
    positioning quickly.
2.  Homepage content prioritizes capabilities and selected evidence.
3.  The project catalogue loads from JSON.
4.  Search and filters work correctly.
5.  Each project detail page renders the available project information.
6.  External links and embeds work or fail gracefully.
7.  The site is responsive and accessible.
8.  No placeholder project is presented as genuine completed work.
9.  No private content or credentials are exposed.
10. The website is deployed and the public URL is verified.

------------------------------------------------------------------------

## 18. Immediate next task: homepage visual prototype

Create a homepage prototype first, not the complete application.

Use a small set of clearly labelled fictional/sample projects to
demonstrate the intended card and case-study presentation. Do not invent
achievements or imply sample projects are Devank's actual work.

Deliver: - A brief design rationale. - One polished homepage layout. -
Responsive desktop and mobile behavior. - Reusable typography, color and
spacing tokens. - Navigation, hero, selected-work cards, capability
section, tools overview, currently-building section and footer. - A
short list of assumptions and open questions.

Do not build the full catalogue, backend, admin system or deployment
workflow during this first task. Obtain review and approval of the
homepage direction before expanding the implementation.
