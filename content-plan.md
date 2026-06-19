# Content Plan

Initial content plan for `UWC ML Liaison Notes`.

## First Blog Posts

### 1. Introducing The UWC ML Liaison Role

Purpose:
- explain why the role exists
- describe the three workstreams
- introduce the blog as a public working notebook
- invite contact from people working on MLWP

Core points:
- MLWP is moving fast, but operational use requires shared understanding,
  verification, and infrastructure.
- UWC institutions face overlapping questions and should not solve all of them
  separately.
- The role focuses on frontier understanding, benchmarking/verification, and
  data-sharing/co-development.
- The blog will report useful synthesis, not private meeting notes.

Possible structure:
- Why this role exists
- The three workstreams
- What this blog will cover
- How to get involved

### 2. Announcing The Physical-Process MLWP Seminar Series

Purpose:
- launch the seminar series
- explain why physical-process-focused discussion is needed
- invite speakers and participants

Core points:
- headline MLWP scores are not enough
- the community needs to ask whether models represent atmospheric processes
- each seminar should focus on one process, one modelling/evaluation approach,
  findings, and transferability
- likely themes include precipitation, clouds, convection, dynamical balance,
  physical consistency, uncertainty, and data assimilation

Source material:
- `../Physical-process MLWP seminar series/README.md`

### 3. Why Physical-Process Verification Matters For MLWP

Purpose:
- explain the scientific motivation behind process-oriented verification

Possible hook:
- physically motivated constraints can improve specific regimes, but are not the
  same as full process understanding

Core distinction:
- targeted constraints can fix known model behaviours
- process understanding asks whether the model reproduces the mechanism and its
  scale interactions

Useful examples:
- AIFS light-precipitation regime separation from Moldovan et al. 2026
- Hauke Schulz's LES/GNN shallow-convection work

### 4. Towards Common Verification Tooling For MLWP

Purpose:
- describe the RMI/KNMI/AEMET/DMI tooling direction
- explain why common data formats and reusable verification workflows matter

Core points:
- verification should not be rebuilt separately at each centre
- common data structures make comparison and shared tooling possible
- operations-focused evaluation needs both classical scores and process-aware
  diagnostics

Source material:
- `../MLWP verification/`
- `../../Planning/2026-04-30-outline.md`

### 5. What Does A Km-Scale MLWP Benchmark Need To Test?

Purpose:
- open the benchmark discussion
- distinguish headline scores, operational usefulness, extremes, physical
  consistency, and process behaviour

Core questions:
- What variables and domains matter?
- Which lead times and weather regimes matter?
- How should extremes and rare events be treated?
- How should physical consistency be evaluated?
- What would make a benchmark useful to operational meteorological services?

### 6. The Current Software Ecosystem For ML Weather Forecasting

Purpose:
- map the software, model, data, and tooling ecosystem emerging around MLWP
- identify what is reusable, what is fragmented, and where common infrastructure
  could help meteorological services

Core questions:
- Which model frameworks, trained models, datasets, and tooling projects are
  becoming important?
- Which parts of the stack are mature enough for operational experimentation?
- Where are centres duplicating effort?
- What does the ecosystem make easy, and what does it make difficult?
- What should UWC track or support as shared infrastructure?

Source material:
- `../../Coordination/earthsci-ml-ecosystem/`
- `../../Tracking/Logbook/2026-05-07.md`

## Core Pages

### Home

Draft opening:

> Machine-learning weather prediction is moving quickly. This site documents
> work from the UWC ML Liaison role to help meteorological services understand
> the scientific frontier, develop common verification approaches, and build
> practical collaboration around data, tools, and physical-process
> understanding.

Must include:
- role description in one paragraph
- three focus areas
- links to Blog, Projects, Seminar Series, Contact

### About

Must include:
- who Leif is
- what the UWC ML Liaison role is
- what UWC is, at a high level
- clarification that the site is not an official E-AI website
- invitation to contact Leif

### Projects Index

Initial projects:
- Physical-Process MLWP Seminar Series
- Common MLWP Verification Tooling
- Km-Scale MLWP Frontier / Review
- MLWP Data Sharing And Common Formats
- MLWP Ecosystem Map, if suitable for public release

### Seminar Series

Use material from:
- `../Physical-process MLWP seminar series/README.md`

Must include:
- purpose
- seminar format
- key questions for speakers
- candidate themes
- how to suggest a speaker/topic

Do not publish named speakers as confirmed unless they have agreed.

### Resources

Start small. Include only durable, public resources.

Initial categories:
- MLWP review/frontier
- verification and benchmarking
- data formats and tooling
- physical-process evaluation
- community initiatives

### Contact

Keep minimal:
- email
- what kinds of input are welcome
- note that suggestions for seminar speakers and papers are welcome

## Publication Safety Checklist

Before publishing a post or page, check:
- Does it quote private email or meeting content without permission?
- Does it imply someone has agreed to speak or collaborate when they have not?
- Does it attribute a position to an institution rather than an individual?
- Does it disclose unpublished work, model names, or internal plans?
- Does it overstate what a paper or conversation proves?
- Is the distinction clear between Leif's interpretation and official UWC/E-AI
  positions?

## Launch Content Checklist

Minimum viable public launch:
- Home page
- About page
- Blog index
- first blog post: `Introducing The UWC ML Liaison Role`
- Projects index
- Seminar Series page
- Contact page

Nice to have, but not required:
- second blog post announcing seminar series
- Resources page
- tags
- RSS
- search
- comments
