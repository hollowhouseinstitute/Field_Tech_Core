# Tests — Field Tech Core

Automated validation and compliance checks for **Field Tech Core**.

These tests make sure that anything running in the field behaves the way the
Hollow House Institute expects around **data integrity, co-regulation tagging,
and ethical safeguards**.

---

## What is covered

- **Unit tests** using `pytest`  
  - core helpers and utilities  
  - event parsing and tagging functions  
  - adapters / IO helpers

- **Schema validation for datasets**  
  - required fields present  
  - correct types and ranges  
  - timestamp and ID conventions

- **Ethical compliance assertions**  
  - redaction / masking of sensitive content  
  - blocking of disallowed actions or states  
  - enforcement of Flame License + Standards Library rules where applicable

---

## Running tests locally

From the repo root:

```bash
pip install -r requirements-dev.txt   # when this file exists
pytest -v
pytest SRC/Tests/test_event_streams.py -v
