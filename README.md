## Hi, I'm Jinjong Mo

Data Engineer at **rsquare** (DS Team)

Building data pipelines in PropTech / government / real estate domain.

### Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazonwebservices&logoColor=white)
![Airflow](https://img.shields.io/badge/Airflow-017CEE?style=flat&logo=apacheairflow&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat&logo=duckdb&logoColor=black)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat&logo=kotlin&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat&logo=springboot&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)

**AWS**: S3, RDS (Aurora), Batch, ECR, IAM, Step Functions

**Backend**: Kotlin/Spring Boot, FastAPI

**Data**: Polars, DuckDB, PostgreSQL, Oracle, DB2, Vertica

**Infra**: Docker, GitHub Actions

### Certifications

| AWS | Data |
|-----|------|
| Solutions Architect Associate (SAA) | ADsP |
| Developer Associate (DVA) | |
| Data Engineer Associate (DEA) | |
| Machine Learning Associate (MLA) | |

### Experience

**Reverse Engineering & Network-level Automation** (2023-2025, 1,100+ commits, solo)
- Selenium + pywinauto on Windows RDP with mandatory security software
- Custom print server to bypass print solution restrictions (physical printer only)
- SQS/DynamoDB integration, payment module with retry strategies
- pytest: unit / integration / E2E test suite

**Serverless Data Pipeline** (2026~)
- EventBridge Scheduler → Step Functions → AWS Batch (Fargate arm64) → S3
- Collect (JSONL.gz) → DuckDB normalize (Parquet) → master table build → RDS import
- S3 PUT 85,000 → 240 per run (99.7% reduction)
- DuckDB httpfs for direct S3 Parquet query without download
- Airflow 3.x DAG orchestration

**Distributed Processing** (2024)
- Ray cluster for event change monitoring (100K+ parallel processing)
- Polars + Ray distributed pipeline → file-based writer separation

**PDF Parser**
- 4-phase pipeline for 5 document types, 400K+ documents with 0% error rate
- Packaged as installable Python library, pytest coverage

**Large-scale Data Ingestion**
- Public API: 250M+ records collected and loaded to RDS
- Geospatial SHP 2.77TB, CSV 1TB to S3/RDS
- Document PDFs: 815K files (650GB) to S3

**Ops & Tooling**
- FastAPI ops dashboard, OpenTelemetry log forwarder PoC
- Introduced pre-commit (ruff + mypy) for code quality across team repos
- Adopted uv as Python project/dependency manager
