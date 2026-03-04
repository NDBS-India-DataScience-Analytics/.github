# POC / Use Case Submission Checklist

Use this checklist before marking a repo as **Demo-ready** and adding it to the Hub Catalog.

## A) Repo Basics (must)
- [ ] Repo name follows convention: `poc-<team>-<short-name>` or `uc-<team/domain>-<short-name>`
- [ ] Repo is under the org: `NDBS-India-DataScience-Analytics`
- [ ] Repo visibility is correct (Private) and access is given only to the owning team (if strict visibility is required)
- [ ] `main` branch protected (PR required + at least 1 approval)
- [ ] `.github/CODEOWNERS` present and points to owning team

## B) Documentation (must)
- [ ] `README.md` includes:
  - [ ] Problem statement + objective
  - [ ] What the POC does (scope + non-scope)
  - [ ] Architecture (high level)
  - [ ] Setup steps (local)
  - [ ] How to run (commands)
  - [ ] Demo steps (what to show + expected output)
  - [ ] Owners (primary + backup) + team
  - [ ] Status + last updated date
- [ ] `docs/` includes (at least one):
  - [ ] `architecture.md` or `design.md`
  - [ ] `limitations.md` (known issues, assumptions)

## C) Reproducibility (must)
- [ ] Dependency file present: `requirements.txt` or `pyproject.toml`
- [ ] `.env.example` exists (no real secrets committed)
- [ ] A single “one command” entry exists:
  - [ ] `scripts/run_demo.py` OR `make demo` OR `docker compose up` (any one)

## D) Security & Compliance (must)
- [ ] No secrets committed (keys/passwords/tokens)
- [ ] No sensitive data committed (customer/PII/confidential datasets)
- [ ] Large files not committed (datasets/models). Use links or storage and document access steps.

## E) Quality (recommended)
- [ ] Basic smoke test or minimal unit tests in `tests/`
- [ ] Logging added for key steps
- [ ] Clear error messages for missing env vars / missing files
- [ ] Release tag created for demo version: `v1-demo` (or similar)

## F) Hub Catalog Update (must)
- [ ] Added/updated entry in Hub Catalog with:
  - Repo link
  - Owner(s)
  - Team
  - Status
  - Short description
  - Stack (tools)
  - Last updated date
