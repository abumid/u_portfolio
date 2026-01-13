# Project 1: Relational Database Design (Quick-Service Restaurant)

## Overview
Designed and implemented a relational SQL database to support restaurant operations including customer orders, order details, payments, employees, scheduling, inventory supplies, and customer feedback.

## What’s included
- **Schema design** (tables, keys, constraints)
- **Data population** scripts
- **Import/Export** scripts
- **ER/EER diagrams** for conceptual and logical design

## Repository structure
- `assets/` — ER/EER and database diagrams
- `sql/` — SQL scripts (create, insert, import/export, drop)
- `data/` — sample dataset used for loading/import

## Diagrams
![Database Diagram](assets/db-diagram.jpg)

![EER Diagram](assets/eer-diagram.jpg)

## How to run (typical flow)
1. Run `sql/01_create_tables.sql`
2. Run `sql/02_insert_data.sql` (or use import script if needed)
3. Use `sql/03_import.sql` and `sql/04_export.sql` as required
4. To reset the database, run `sql/05_drop_tables.sql`
