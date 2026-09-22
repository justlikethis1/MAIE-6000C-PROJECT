# Week 03 Individual Readiness Lab

## Required Tag

`w03-readiness`

## What I Changed

- Added an integration test for requesting a case that does not exist.
- The test verifies that the API returns HTTP 404 with the expected `Case not found` detail.

## How I Verified It

- Started the local Docker Compose stack with PostgreSQL, the API service, the AI service, and the worker.
- Ran the focused integration test:
  `python -m pytest tests/integration/test_api_case_flow.py -q`
- Result: `1 passed`.
- The API and AI health endpoints returned status `ok`.

## Reproducibility

- Python environment: `maie6000c-w03`
- Python version: 3.11
- Dependencies are listed in `requirements.txt`.
- Docker Compose provides the local database and service stack.

## AI Use Statement

- Tool: GitHub Copilot
- Used for: understanding the starter repository, selecting a small bounded test change, and drafting this documentation.
- Verified, changed, or rejected: I reviewed the suggested test, included it in the repository, and ran the focused test locally. The test passed.
