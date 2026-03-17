# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a single-page interactive scrollytelling visualization (Dutch language) that demonstrates how flat tabular data transforms into a knowledge graph (ontology). The domain is a healthcare case study about patient referral processes between a hospital (Ziekenhuis A) and a rehabilitation center (Zorggroep B) for geriatric rehabilitation care (GRZ).

## Architecture

The entire application lives in a single `index.html` file with no build system, bundler, or package manager. To run it, open `index.html` directly in a browser.

**External dependencies (loaded via CDN):**
- Tailwind CSS (via `cdn.tailwindcss.com`) — utility-first styling
- D3.js v7 (via `d3js.org`) — force-directed graph visualization

**Key sections in `index.html`:**
- **`<style>`** — Custom CSS for scrollytelling layout (sticky figure, step cards), table styling, and D3 node/link appearance
- **`<header>`** — Introductory context section explaining the healthcare case
- **`<section id="scrolly">`** — Two-column layout: left `<article>` with 5 scroll steps (`data-step="0"` through `data-step="4"`), right `<figure>` with the HTML table and D3 SVG canvas
- **`<script>`** — All application logic:
  - `tableData` / `graphData` — static data definitions (nodes, links, properties)
  - D3 setup: SVG, force simulation, node/link rendering, drag behavior
  - `steps[]` array — 5 functions (step0–step4) controlling what's visible at each scroll position
  - `IntersectionObserver` — triggers step functions based on scroll position

**Scrollytelling flow (5 steps):**
1. Step 0: Flat HTML table visible
2. Step 1: Table cells morph into colored D3 nodes (entities)
3. Step 2: Property labels appear on nodes
4. Step 3: Relationship edges (links with labels) appear between nodes
5. Step 4: D3 force simulation activates — nodes become draggable

**Color scheme:** Blue (#3b82f6) = Hospital, Green (#10b981) = Care group, Purple (#a855f7) = Management
