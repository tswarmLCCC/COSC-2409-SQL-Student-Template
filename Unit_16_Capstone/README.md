
    "README.md": "# COSC 2409: Enterprise Data Engineering\n\nWelcome to the COSC 2409 Capstone environment. This repository serves as the professional portfolio piece for your final project, where you will demonstrate mastery of the entire data engineering lifecycle.",
    ".devcontainer/devcontainer.json": '{\n  "name": "COSC 2409 Capstone",\n  "image": "mcr.microsoft.com/devcontainers/base:ubuntu",\n  "postCreateCommand": "sudo apt-get update && sudo apt-get install -y postgresql && sudo service postgresql start && sudo -u postgres psql -c \\"ALTER USER postgres PASSWORD \'postgres\';\\" && sudo -u postgres createdb cosc2409"\n}',
    "Unit_16_Capstone/README.md": """# Capstone Project: DataCo Global Logistics Engine

## Mission
You are the lead Data Architect for DataCo Global Logistics. The organization is currently suffering from operational paralysis due to a massive, redundant flat-file data dump. Your task is to transform this raw chaos into a high-speed, secure, and predictive intelligence engine.

## Architectural Requirements
You are not just writing queries; you are building an engine. Your work will be evaluated on the following:

1. **Relational Integrity (3NF):** You must eliminate all data redundancies. If a table contains repeating groups or multi-valued attributes, your schema is flawed.
2. **Performance Optimization:** Use `EXPLAIN ANALYZE` to verify your query paths. Implement B-Tree indexes on high-traffic foreign keys and lookup columns to ensure sub-second response times.
3. **Advanced Analytical Logic:** Your `v_supply_chain_intelligence` view must utilize:
   - **CTEs** to modularize your data staging.
   - **Window Functions** to perform trend analysis (Running Totals, Moving Averages).
   - **CASE Statements** to standardize business logic and categorize risk.
4. **AI Grounding:** Integrate MindsDB to provide predictive insights. You must document the `_confidence` score of your predictions—an AI insight without a confidence metric is a liability in a business environment.

## Documentation Standards (The Data Dictionary)
20% of your final grade is determined by your `Data_Dictionary.md`.
- Explain the **business rules** behind your CASE statements.
- Define the semantic meaning of every column.
- If another engineer cannot understand your data architecture without asking you for a meeting, your documentation is insufficient.

## Deliverables
- `init_schema.sql`: The complete architectural script.
- `Data_Dictionary.md`: The technical blueprint of your system.""",
    "Unit_16_Capstone/init_schema.sql": "-- ==========================================\n-- WEEK 16 CAPSTONE: Global Logistics\n-- ==========================================\n\n-- STEP 1: ARCHITECTURE (DDL)\n-- Create your 3NF tables: Locations, Customers, Products, and Orders.\n\n\n-- STEP 2: DATA MIGRATION (DML)\n-- Populate your tables using INSERT INTO ... SELECT DISTINCT from 'raw_staging'.\n\n\n-- STEP 3: OPTIMIZATION\n-- Create B-Tree indexes on high-traffic columns.\n\n\n-- STEP 4: ADVANCED ANALYTICS\n-- Create 'v_supply_chain_intelligence' using Window Functions and CASE.\n\n\n-- STEP 5: AI INTEGRATION (MindsDB)\n-- CREATE PREDICTOR and query it for future delivery risks.",
    "Unit_16_Capstone/Data_Dictionary.md": "# Data Dictionary\n\nDocument your 3NF schema and the logic behind your analytical transformations.
