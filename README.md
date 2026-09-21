# GitHub Skills Challenge

This repository contains a small Python application and a GitHub Actions CI setup for running tests and coverage checks.

## Project overview

- Python application code lives under the `src` directory.
- Tests live under the `tests` directory.
- GitHub Actions workflows live under `.github/workflows`.

## Local verification

Create and activate a virtual environment, then run:

```bash
source .venv/bin/activate
PYTHONPATH=. pytest -vv -ra --cov=src --cov-report=term-missing
```

## CI workflows

- `.github/workflows/python-package.yml` runs the Python test suite on pull requests to `main`.
- `.github/workflows/python-coverage.yml` runs coverage analysis and enforces a minimum coverage threshold.

## Notes

This repository is set up for GitHub Actions-based validation and continuous integration checks.

