# Capstone Project: DataCo Global Logistics Engine

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
- `Data_Dictionary.md`: The technical blueprint of your system.
