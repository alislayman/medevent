# MedOnField — product documentation

Public documentation for **MedOnField**, a two-sided marketplace connecting
medical professionals (doctors, nurses, officials, cutmen, ambulance staff)
with event organisers who need qualified on-site medical coverage.

**[Open the documentation →](https://alislayman.github.io/medevent/)**

## What's in this repository

| File | Purpose |
| --- | --- |
| `index.html` | Landing page. Links to the two documents below. |
| `specification.html` | The full product specification and agreed project scope — roles, data model, key flows, admin panel, roadmap and pricing. |
| `timeline.html` | Project timeline. Every feature with its status across development, test and production, plus progress bars and the external services the project depends on. |
| `.nojekyll` | Tells GitHub Pages to serve the files as-is, without Jekyll processing. |

Each document is a single self-contained HTML file. Diagrams in the
specification render client-side with [Mermaid](https://mermaid.js.org/) from a
CDN, so there is no build step — open any of them in a browser to preview
locally.

## Updating the timeline

All state lives in one editable block at the top of the `<script>` in
`timeline.html`, marked `EDIT BELOW THIS LINE`. Change a status, commit, and the
progress bars recalculate on their own — nothing is computed by hand.

- **Development:** `ready` · `progress` · `done`
- **Test and production:** `none` · `needs` · `tested`
- **Environment hosting:** set `hosted: true` on an entry in `ENVIRONMENTS` once it is live.

External dependencies are counted alongside features in every progress bar, so
an environment cannot read as complete while a service it needs is still
missing.

## Current revision

**Rev. 3 — 30 July 2026.** Incorporates the client meeting of 29 July 2026 and the follow-up notes of 30 July 2026;
section 23 lists every item agreed in that meeting, where each one is
specified, and the phase it falls in. Supersedes the draft of 11 July 2026.

## Application code

The application source — Django/DRF backend, React admin panel, Next.js
frontend and devops configuration — lives in a separate **private**
repository, `medonfield`.

## Before you commit

This repository is **public**. Everything committed to `main` is
world-readable while GitHub Pages is enabled. Credentials, test fixtures,
internal notes and client correspondence belong in the private repository.
