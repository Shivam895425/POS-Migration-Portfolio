# POS Migration Lab

An end-to-end POS data migration workflow built with synthetic and public data:

**Extract** (REST API) -> **Transform** (Python + pandas) -> **Load** (DuckDB) -> **Reconcile** (SQL)

> Work in progress. No real merchant or client data is used in this project.

## Stages

- [ ] Stage 1 - Reconcile: SQL checks comparing source and migrated target data
- [ ] Stage 2 - Transform: pandas conversion to a target import format with a validation report
- [ ] Stage 3 - Extract: pull data from a POS sandbox through a REST API
- [ ] Documentation: mapping specification and migration runbook

## Project structure

| Folder | Purpose |
|---|---|
| `config/` | Field mapping configuration |
| `data/sample/` | Small synthetic sample files |
| `data/output/` | Generated files (not committed) |
| `docs/` | Mapping specification and runbook |
| `sql/` | Profiling and reconciliation queries |
| `src/` | Python scripts |

## Requirements

- Python 3.11+
- Packages in `requirements.txt`: `pip install -r requirements.txt`
