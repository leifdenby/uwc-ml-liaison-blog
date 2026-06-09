# UWC ML Liaison Blog

Project plan for a role-branded public blog and lightweight website documenting
Leif Denby's work as UWC ML Liaison.

## Working Title

UWC ML Liaison Notes

## Tagline

A public working notebook on machine-learning weather prediction, verification,
physical processes, and collaboration across UWC.

## Purpose

Create a public working hub for the UWC ML Liaison role.

The site should communicate:
- what the UWC ML Liaison role is for
- what work is underway on machine-learning weather prediction (MLWP)
- what Leif is learning from conversations across UWC, E-AI, ACCORD, and related
  communities
- what collaboration opportunities are emerging
- how projects such as verification tooling, km-scale MLWP review work, data
  sharing, and the physical-process seminar series are developing

The site is not intended to be:
- an official E-AI website
- a formal UWC governance site
- a complete technical documentation portal
- a public dump of private weekly status notes or meeting records

## Positioning

The site is role-branded rather than personal-branded.

Leif should be visible as the author and point of contact, but the primary
identity is the UWC ML Liaison role. This avoids making the site feel like a
generic personal blog, while also avoiding the implication that it is an official
E-AI website or formal UWC governance channel.

Suggested homepage framing:

> Machine-learning weather prediction is moving quickly. This site documents
> work from the UWC ML Liaison role to help meteorological services understand
> the scientific frontier, develop common verification approaches, and build
> practical collaboration around data, tools, and physical-process
> understanding.

## Audience

Primary:
- scientists and technical staff at UWC institutions
- MLWP-interested people in national meteorological services

Secondary:
- E-AI, ACCORD, WMO, and wider weather/ML researchers
- stakeholders interested in operational use of MLWP

## Relationship To Existing Workspace

Private/internal tracking remains in:
- `../../Tracking/status.md`
- `../../Tracking/todo.txt`
- `../../Tracking/Logbook/`

The blog should synthesize selected material from those files, but not expose
private meeting notes, contact details, unconfirmed commitments, or sensitive
institutional positions.

Relevant source material lives in:
- `../../Planning/2026-04-30-outline.md`
- `../Physical-process MLWP seminar series/README.md`
- `../MLWP verification/`
- `../../Communication/`
- `../../Knowledge/`

## Site Structure

### Home

Purpose:
- explain the UWC ML Liaison role
- introduce the main workstreams
- point readers to blog posts and project pages

Sections:
- short introduction
- current focus areas
- featured projects
- latest posts
- contact link

### Blog

Purpose:
- regular public synthesis of work, insights, and open questions

Post types:
- monthly updates
- project announcements
- synthesis from conversations
- technical reflections
- open questions for the community
- seminar summaries

Suggested tags:
- `frontier`
- `verification`
- `benchmarking`
- `data-sharing`
- `physical-processes`
- `seminars`
- `community`
- `operations`

### Projects

Stable project pages for:
- Physical-Process MLWP Seminar Series
- Common MLWP Verification Tooling
- Km-Scale MLWP Frontier / Review
- MLWP Data Sharing And Common Formats
- MLWP Ecosystem Map, if this becomes public-facing

### Seminar Series

Dedicated page linked from Projects.

Use the existing project:
- `../Physical-process MLWP seminar series/README.md`

Include:
- purpose
- speaker format
- key questions for each presentation
- upcoming seminars
- past seminars
- how to suggest a speaker or topic

### Resources

Curated links:
- papers
- benchmark efforts
- verification tools
- data-format discussions
- community initiatives

### About

Purpose:
- describe Leif's role and background
- explain UWC and the ML Liaison remit
- clarify that the site is a working blog, not an official E-AI site

Include:
- what the role is
- why MLWP needs coordination
- how people can engage

### Contact

Simple contact page:
- email
- invitation to suggest papers, projects, seminar speakers, or collaboration
  ideas

## Navigation

Recommended primary navigation:
- Home
- Blog
- Projects
- Seminar Series
- Resources
- About
- Contact

## Editorial Principles

The blog should be:
- clear
- scientifically careful
- useful to peers
- candid about uncertainty
- focused on synthesis rather than self-reporting

Avoid:
- publishing private email content without permission
- naming people as speakers before they agree
- implying official UWC/E-AI positions unless confirmed
- over-claiming model capabilities from one paper or conversation
- turning weekly status updates into public diary entries

Preferred tone:
- direct
- reflective
- technically grounded
- collaborative
- not promotional

## Technical Setup

Chosen approach:
- Quarto static website built from Markdown / QMD files
- minimal theme
- easy deployment through GitHub Pages or equivalent

Rationale:
- Quarto is well suited to a role-branded scientific blog with project pages,
  figures, technical notes, and possible future notebook-backed posts.

Initial approach:
- static site built from Markdown
- minimal theme
- easy deployment through GitHub Pages or equivalent

## Local Development Server

Quarto is required to preview or render the site.

Check whether Quarto is installed:

```sh
quarto --version
```

If that command is not found, install Quarto from:

<https://quarto.org/docs/get-started/>

From this project folder, start the local development server with:

```sh
quarto preview
```

Quarto will print a local URL, typically something like:

```text
http://localhost:4200/
```

The preview server watches the `.qmd`, `_quarto.yml`, and `styles.css` files and
updates the site as they change.

To build the static site without starting a preview server, run:

```sh
quarto render
```

Rendered output is written to `_site/`, as configured in `_quarto.yml`.

Avoid at launch:
- comments
- complex search
- custom backend
- heavy interactive features

Add later if needed:
- RSS
- tags
- simple search
- GitHub-based comments via giscus

## Launch Scope

Minimum useful launch:
- Home
- About
- Blog index
- first blog post
- Projects index
- Seminar Series page
- Contact

Do not wait for:
- perfect styling
- full archive
- comments
- search
- complete project pages

## Immediate Next Actions

1. Install Quarto or use an environment where `quarto` is available.
2. Run `quarto render` in this folder and fix any render issues.
3. Decide URL and repository location.
4. Draft first blog post.
5. Draft seminar-series announcement post.
6. Create project pages from existing README material.
7. Decide what existing content is safe to publish.
8. Deploy private preview.
9. Review for institutional sensitivity.
10. Publish.

## Handoff For Next LLM Session

Start in this folder and read:
- `README.md`
- `content-plan.md`
- `../../Planning/2026-04-30-outline.md`
- `../../Tracking/status.md`
- `../Physical-process MLWP seminar series/README.md`

Then render the Quarto site, fix any issues, and draft the first public post.
