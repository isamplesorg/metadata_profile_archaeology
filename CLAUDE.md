# CLAUDE.md

## Project overview

This repository contains SKOS vocabularies (RDF/Turtle) for iSamples archaeology metadata profiles, specifically extensions used with samples registered in OpenContext. It also functions as a GitHub Action that converts SKOS Turtle files to HTML documentation via a pipeline: Turtle → SQLite (navocab) → Markdown (vocab2mdCacheV2) → HTML (Quarto).

GitHub Pages landing page: <http://isamples.org/metadata_profile_archaeology/> — rendered from `docs/readme.md`, deployed from the `gh-pages` branch under `/docs`. `https://isamplesorg.github.io/metadata_profile_archaeology/` 301-redirects to the `isamples.org` URL.

## Repository structure

- `vocabulary/` — Source SKOS Turtle (.ttl) files
- `tools/` — Python processing tools (vocab.py, vocab2mdCacheV2.py, navocab/)
- `docs/` — Generated HTML/Markdown output (deployed to gh-pages)
- `cache/` — SQLite database directory (should be transient)
- `.github/actions/github_action_main.py` — Docker entrypoint for the pipeline
- `.github/workflows/` — GitHub Actions workflow definitions
- `Dockerfile` — Processing container, pinned to `python:3.12-slim`
- `action.yml` — GitHub Action metadata

## Vocabularies

| File | ConceptScheme CURIE |
|------|-------------------|
| `opencontext_material_extension.ttl` | `ocmat:oc_materialsvocab` |
| `opencontext_materialsampleobjecttype.ttl` | `ocspec:oc_spectypevocab` |

## Pipeline fixes applied 2026-04-22

This repo shares the same codebase as the other `metadata_profile_*` repositories (derived from isamplesorg/vocabularyTemplate). The following fixes were ported from the earth_science repo's 2026-04-22 cleanup:

1. **Dockerfile**: pinned to `python:3.12-slim` so `pkg_resources` remains available (Python 3.14 drops it).
2. **tools/requirements.txt**: added `setuptools<81` (rdflib-sqlalchemy needs `pkg_resources`).
3. **Workflow filename**: `process_vocab.yml` now references `opencontext_materialsampleobjecttype` (was the nonexistent `opencontext_materialsampletype`).
4. **github_action_main.py**: resets the cache DB before each vocabulary (fresh DB per vocab, no cross-vocab pollution); processes load + render per vocab in one pass instead of two separate loops.
5. **vocab2mdCacheV2.py**: `getVocabRoot` now UNIONs `skos:topConceptOf` and `skos:hasTopConcept`; `getNarrower` falls back to an unscoped `skos:broader` query when concepts omit `skos:inScheme`.
6. **navocab.purge_store**: no longer crashes on undefined `graph` local; logs a warning and defers to external file deletion.
7. **.gitignore**: expanded to cover `.claude/`, `.venv/`, `/testoutput/local_run/`, and `tools/navocab/__pycache__/`.

Note: unlike the earth_science and biology repos, this one did **not** have a stale `cache/vocabularies-SMR-Samsung.db`, and the `theindex=0`-inside-loop bug from earth_science was already absent here (index initialized outside the loop).

## GitHub Actions workflows

- **Process vocabularies** (`process_vocab.yml`) — Manual dispatch. Processes both vocabularies.
- **Test docs** (`testdocs_process_vocab.yml`) — Manual dispatch. Test workflow.
- **Test JSON** (`testjson_process_vocab.yml`) — Manual dispatch. JSON generation test.

## Processing pipeline

Same as the earth_science and biology repos:
1. `vocab.py load <file.ttl> <conceptscheme-uri>` — parse Turtle, store in SQLite
2. `vocab2mdCacheV2.py <db> <conceptscheme-uri>` — query DB, generate Markdown
3. `quarto render <file.md> -t html` — render Markdown to HTML
4. Deploy HTML to gh-pages via JamesIves/github-pages-deploy-action
