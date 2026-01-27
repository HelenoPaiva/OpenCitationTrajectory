# Open Citation Trajectory

An open, reproducible report of how scholarly articles are cited over time.

**Live site (GitHub Pages):** https://helenopaiva.github.io/OpenCitationTrajectory/


## What it does

Paste a DOI (or DOI URL) and get:

- Article metadata (Crossref)
- List of citing works (OpenCitations COCI)
- Citations-by-year “trajectory” (from OpenCitations `creation` dates)
- A global citation count reference (OpenAlex `cited_by_count`)
- A one-click Google Scholar search link (no scraping)

## Data sources

- **OpenCitations COCI** — citation links (citing/cited DOI pairs)
- **Crossref REST API** — bibliographic metadata enrichment
- **OpenAlex API** — `cited_by_count` for the target DOI
- **Google Scholar** — provided as a *search link only* (no automated collection)

> Coverage differs across sources. Google Scholar is often higher; this project intentionally stays open and API-based.

## How to run locally

Just open `index.html` in your browser.

## Deploy to GitHub Pages

1. Push `index.html` (and this `README.md`) to `main`
2. GitHub → **Settings → Pages**
3. **Source:** Deploy from branch
4. **Branch:** `main` / root

## Notes & limitations

- OpenCitations doesn’t cover all publishers/venues; some citing works may be missing.
- Crossref enrichment is limited to the **first N DOIs** (configurable in Settings) to keep requests reasonable.
- Citation-by-year is computed from OpenCitations `creation` dates (not publication year).

## License

This repository is intended for open academic use.  
License terms will be finalized prior to any commercial deployment.


## Author

**Heleno de Paiva Oliveira, MD, PhD**  
Professor of Anesthesiology  
Universidade Federal do Rio Grande do Norte (UFRN), Brazil
