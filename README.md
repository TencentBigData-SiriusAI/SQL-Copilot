# SQLGovernor: Towards an LLM-powered SQL Toolkit for Real World Application
[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

## 📖 Overview
This repository accompanies the paper **SQLGovernor: Towards an LLM-powered SQL Toolkit for Real World Application** and provides:

###  Payment-SQL Dataset

Table 1: Detailed Statistics on Payment-SQL
| Data Statistics           | Value |
|---------------------------|-------|
| # SQL Queries             | 50    |
| # Average Tables          | 2     |
| # Average Columns         | 11    |
| Average Token Length      | 421   |
| Max Token Length          | 1169  |
| Min Token Length          | 163   |


#### Key Observations
- Industrial-level Complexity:
  -  Average token length (421) far exceeds academic benchmarks (e.g., BIRD's 107 tokens).
  - Longest query spans 1,169 tokens, reflecting real-world nested operations.

- Realistic Schema Interactions:
  - Queries involve 2 tables and 11 columns on average, mirroring production-grade JOIN patterns.

- Rigorous Evaluation Baseline:
  - Minimum token length (163) still surpasses Spider 2.0’s "difficulty threshold" (160 tokens).
  - For research use, this dataset benchmarks SQL optimization tools under industrial-grade complexity.

### Framework Design

<img src="architecture.png" alt="System Architecture" style="zoom: 100%;" /> 

#### SQL Toolkit

- Include four carefully deisgned tools, i.e., SQL Rewriter, SQL Modifier, Syntax Error Corrector, Equivalence Verifier.

#### Knowledge Management

- Include specialized knowledge bases supported by self-evolving mechanism.


