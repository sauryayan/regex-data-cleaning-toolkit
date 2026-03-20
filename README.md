# Regex Data Cleaning Toolkit: Parsing Unstructured Logs

## Overview
Real-world data is rarely cleanly formatted in relational tables. This project demonstrates the ability to extract structured, actionable data from chaotic, unstructured text using **Python** and **Regular Expressions (Regex)**. 

This toolkit was developed by processing a mock "Customer Support Log" containing a deliberate mix of inconsistent formats, simulating the messy realities of vendor CRMs and legacy databases. 

## The Challenge
The goal of this project was to write highly specific, non-greedy Regex patterns to parse a dense text block and successfully extract 30 distinct data points without capturing false positives.

**Data extracted includes:**
* **Financials:** Currency amounts with and without symbols.
* **Temporal Data:** Dates in various formats (ISO, US, dot-separated) and 12/24-hour timestamps.
* **Contact Information:** Emails, domains, and four distinct international and domestic phone number formats.
* **System Identifiers:** Order numbers, Transaction IDs, Error Codes, and Customer IDs.

## Skills Demonstrated
* **Advanced Regular Expressions:** Character classes, quantifiers, anchors, and capture groups `()`.
* **Pattern Optimization:** Utilizing the OR operator `|` and precise digit counts `{n}` to prevent greedy matching (e.g., ensuring a date is not falsely identified as a phone number).
* **Data Masking:** Implementing substitution logic to redact sensitive PII (like email addresses) from text logs.
* **Python:** String manipulation and pattern extraction.

## Files in this Repository
* `Regex_Data_Cleaning_Gauntlet.ipynb`: The core Jupyter Notebook containing the raw unstructured text, the documented Regex patterns, and the execution output.

## Author
**Sauryayan Ralhi** *Data Analyst*

---
*Note: This repository serves as a lightweight utility demonstration, showcasing the foundational data wrangling skills required before heavier analytical work (like correlation matrices or consumer behavior modeling) can begin.*
