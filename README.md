# qap-site-scoring

This project scores sample development sites against LIHTC QAP location criteria. It uses SQLite and plain Python. It ranks the sites and explains how each score was earned.

This is a work in progress. All data in this repo is sample data.

## Project plan

* Store QAP scoring rules in a database table, not in code.
* Version the rules by state and year.
* Keep site points separate from application points.
* Calculate straight line distance from each site to nearby amenities.
* Rank the sites and show a breakdown of each score.
* Document every assumption, such as distance method and tie handling.

## Folder layout

* `data/` holds sample sites, sample amenities, and rule files.
* `sql/` holds the database schema and the scoring queries.
* `src/` holds the Python scripts.
* `tests/` holds the unit tests.
