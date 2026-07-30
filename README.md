# MedOnField — product documentation

Public documentation for **MedOnField**, a two-sided marketplace connecting
medical professionals (doctors, nurses, officials, cutmen, ambulance staff)
with event organisers who need qualified on-site medical coverage.

**[Read the specification →](https://alislayman.github.io/medevent/)**

## What's in this repository

| File | Purpose |
| --- | --- |
| `index.html` | The full product specification and agreed project scope — roles, data model, key flows, admin panel, roadmap and pricing. Published via GitHub Pages. |
| `.nojekyll` | Tells GitHub Pages to serve the file as-is, without Jekyll processing. |

The document is a single self-contained HTML file. Diagrams render client-side
with [Mermaid](https://mermaid.js.org/) from a CDN, so there is no build step —
open `index.html` in a browser to preview it locally.

## Current revision

**Rev. 2 — 30 July 2026.** Incorporates the client meeting of 29 July 2026;
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
