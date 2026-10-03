# SQL for Beginners: Hands-On Colab Lab

A self-contained, beginner-level SQL lab that runs in Google Colab with no installation. It supports the MSDS 525 Final Project (traffic congestion near Nashville International Airport, BNA) and the AI / Data Science certificate.

**Author:** Pushpita Chatterjee, School of Applied Computational Sciences, Meharry Medical College
**Version:** 1.0 (October 2026)

## What you will learn

| Part | Topics |
| --- | --- |
| DDL | `CREATE TABLE`, constraints (`PRIMARY KEY`, `NOT NULL`, `UNIQUE`, `CHECK`, `FOREIGN KEY`), `ALTER`, `DROP`, indexes |
| DML | `INSERT`, `UPDATE`, `DELETE`, loading many rows |
| Querying | `SELECT`, `WHERE`, `ORDER BY`, `LIMIT`, `DISTINCT`, `LIKE`, `IN`, `BETWEEN`, `IS NULL` |
| Functions | Aggregate, text, number, date/time, `COALESCE`, `CASE`, `CAST` |
| Grouping | `GROUP BY`, `HAVING` |
| Joins | `INNER`, `LEFT`, `RIGHT`/`FULL` (where supported), `CROSS`, self join, and the fan-out trap |
| Advanced | Subqueries, CTEs, views, window functions, set operations, transactions |
| Practice | 7 exercises with solutions, and a route map for the BNA project |

## How to run

1. Open Google Colab (colab.research.google.com).
2. Choose **File > Upload notebook** and select `SQL_for_Beginners_Colab.ipynb`.
3. Choose **Runtime > Run all**, or run cells in order with Shift+Enter.
4. If you see "UNIQUE constraint failed" or "table already exists", a cell was run twice. Choose **Runtime > Restart and run all**.

No files or accounts other than a Google account are needed.

## Important notes

- **Database engine:** the lab uses SQLite, which is built into Python. The course project uses MySQL. The SQL logic is the same; the notebook includes a SQLite-vs-MySQL cheat sheet for the differences (date functions, `||`, `CREATE OR REPLACE VIEW`, `DESCRIBE`).
- **Sample data is synthetic.** The incidents, weather and flight tables in the notebook are randomly generated with a fixed seed. They are for learning only and must **not** be cited as real findings.
- **Real data** for the project is described in the assignment and in the separate data pack README.
- Colab's SQLite version may be older than the one this was tested on; `RIGHT JOIN` and `FULL JOIN` cells are guarded and print a message instead of failing.

## Files

| File | Purpose |
| --- | --- |
| `SQL_for_Beginners_Colab.ipynb` | The lab notebook |
| `README.md` | This file |
| `LICENSE` | MIT License |

## License

The notebook and this README are released under the MIT License (see `LICENSE`). You may use, adapt and share them with attribution.

Data sources used in the project (not included in this lab) have their own terms:
- NOAA National Centers for Environmental Information daily summaries: U.S. government data, generally public domain; cite NOAA NCEI.
- Metro Nashville Open Data (Traffic Accidents): check the license on the dataset page and cite it.
- BNA aviation statistics: published by the Metropolitan Nashville Airport Authority; cite it.

## Citation

Chatterjee, P. (2026). *SQL for Beginners: Hands-On Colab Lab* (v1.0). Meharry Medical College, School of Applied Computational Sciences.

## Feedback

Report errors or suggestions to your course instructor.
