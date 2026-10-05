# 👋 Hi, I'm Shubham Garje

### Data Engineer | Snowflake | dbt | ETL | SQL | Cloud Data Engineering | IICS-CDI | UNIX Scripting | Informatica MDM SaaS | Semarchy xDM

I build **scalable data pipelines, modern data platforms, and metadata-driven ETL solutions** using Snowflake, dbt, SQL, Python, and cloud technologies.

🎯 **Career Focus:** Senior Data Engineer / Snowflake Data Engineer  
💡 **Current Focus:** Modern Data Stack • Snowflake • dbt • Data Engineering  
🚀 **Goal:** Build production-grade data solutions that solve real business problems.

---

## 🛠️ Tech Stack

**Data Engineering**
- Snowflake
- SQL — Oracle | SQL Server | PostgreSQL
- dbt
- Informatica IICS
- ETL / ELT
- SCD Type 1 & Type 2
- CDC & Metadata-driven pipelines

**Cloud & Data Platform**
- AWS S3
- Snowflake Tasks
- Streams
- Snowpipe
- Dynamic Tables
- Zero-Copy Cloning
- Data Sharing
- Micro-partitioning & Clustering

**Programming**
- Python
- Unix / Shell Scripting
- Jinja
- Git / GitHub

**AI & Modern Data**
- Snowflake Cortex
- AI Agents
- Semantic Layer
- Snowpark

---

## 🚀 Featured Projects

### ❄️ Snowflake + dbt Data Engineering Platform
End-to-end modern data pipeline implementing:

- Bronze → Silver → Gold architecture
- dbt transformations
- Incremental models
- SCD Type 2
- Macros & Jinja
- Metadata-driven pipelines
- Data quality & testing
- Snowflake Tasks & Streams

### 🤖 Snowflake Cortex AI Agent
Built an AI-powered data agent on top of Snowflake that allows business users to query enterprise data using natural language.

**Impact:** Reduced repetitive business data requests by enabling self-service analytics.

### ⚙️ Metadata-Driven ETL Framework
Designed reusable ETL logic using metadata/configuration instead of hardcoded pipelines.

**Focus:** Scalability, maintainability and reduced development effort.

## 🚀 Data Engineering Projects

### 1. Modern Data Platform — Snowflake + dbt - with Medallion Architecture 

**Domain:** Analytics / Data Warehouse

**Technology:** Snowflake • dbt • SQL • Jinja • AWS S3 • Git/GitHub

#### Project Flow

```text
                SOURCE SYSTEMS
                     │
                     ▼
              ┌─────────────┐
              │   AWS S3    │
              │ Raw Files   │
              └──────┬──────┘
                     │
                     ▼
              ┌─────────────┐
              │  Snowflake  │
              │ RAW Layer   │
              └──────┬──────┘
                     │
                  dbt
                     │
                     ▼
              ┌─────────────┐
              │   STAGING   │
              │ Cleaning &  │
              │ Standardize │
              └──────┬──────┘
                     │
                  dbt
                     │
                     ▼
              ┌─────────────┐
              │   SILVER    │
              │ Business    │
              │ Transform.  │
              └──────┬──────┘
                     │
                  dbt
                     │
                     ▼
              ┌─────────────┐
              │    GOLD     │
              │ Fact & Dim  │
              │ Models      │
              └──────┬──────┘
                     │
                     ▼
              ┌─────────────┐
              │ BI / AI /   │
              │ Analytics   │
              └─────────────┘
```

#### dbt Implementation

```text
Sources
   │
   ▼
Staging Models
   │
   ├── Data Cleaning
   ├── Renaming
   ├── Type Casting
   └── Standardization
   │
   ▼
Intermediate Models
   │
   ├── Joins
   ├── Business Logic
   └── Reusable Transformations
   │
   ▼
Gold Models
   │
   ├── Fact Tables
   ├── Dimension Tables
   └── Analytics Models
   │
   ▼
BI / Reporting
```

#### Key Implementations

- Built **ELT pipelines** using Snowflake and dbt.
- Implemented dbt **staging, intermediate and mart layers**.
- Developed reusable **Jinja macros** to eliminate repetitive SQL.
- Implemented **metadata-driven transformations** using dbt configuration.
- Implemented **incremental models** for efficient processing of large datasets.
- Implemented **SCD Type 2** to maintain historical dimension records.
- Used Snowflake **Streams and Tasks** for CDC-driven processing.
- Implemented dbt tests for **data quality and integrity**.
- Used Snowflake **micro-partitioning and clustering** for query performance.
- Managed code using **Git/GitHub** with branch-based development.
- Built reusable transformation patterns rather than hardcoding individual pipelines.

**Architecture Focus:**  
`S3 → Snowflake RAW → dbt Staging → Silver → Gold → BI/AI`

---

### 2. Enterprise Customer & Vendor Data Integration Platform

**Domain:** Master Data Management / Logistics

**Technology:** Informatica IICS • SQL Server • PostgreSQL • Semarchy MDM • Snowflake • AWS S3 • SQL • XML/XSD

#### Project Flow

```text
Source Systems
     │
     ▼
┌─────────────────────┐
│ Operational Sources │
│ Customer / Vendor   │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│     OD Layer        │
│ Operational Data    │
└──────────┬──────────┘
           │
        IICS ETL
           │
           ▼
┌─────────────────────┐
│     SA / SD Layer   │
│ Staging / Standard  │
│ & Data Preparation  │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│    Semarchy MDM     │
│ Golden Records      │
│ Customer / Vendor   │
└──────────┬──────────┘
           │
        IICS ETL
           │
           ▼
┌─────────────────────┐
│    AL / Reporting   │
│      Snowflake      │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ AWS S3 / XML Layer  │
│ XSD-based messages  │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────────────┐
│ Downstream Applications     │
│ CargoWise | Breakbulk       │
│ IMPAX | Meridian            │
└─────────────────────────────┘
```

#### Key Responsibilities

- Designed and maintained **end-to-end ETL pipelines** using Informatica IICS.
- Integrated Customer and Vendor data from heterogeneous databases.
- Implemented data standardization and transformation between OD → SA/SD → MDM layers.
- Worked with **Semarchy MDM** for golden-record creation and master-data management.
- Implemented CDC-based processing using MDM-generated update timestamps.
- Built Snowflake-based downstream data processing.
- Integrated Snowflake with **AWS S3** for file-based data exchange.
- Generated XML messages according to defined XSD structures.
- Supported downstream integrations with multiple enterprise applications.
- Troubleshot ETL failures, stored procedures, data-quality issues and production data discrepancies.

**Architecture Focus:**  
`ETL → Data Quality → MDM → Golden Record → Snowflake → Downstream Integration`

---

## 🧠 Advanced Snowflake Implementations

Across these projects, the following Snowflake capabilities were implemented:

```text
Snowflake
│
├── Streams
├── Tasks
├── Dynamic Tables
├── Incremental Processing
├── SCD Type 1 / Type 2
├── CDC
├── Micro-partitioning
├── Clustering
├── Time Travel
├── Zero-Copy Cloning
├── Snowpipe
├── AWS S3 Integration
├── Snowpark
└── Cortex AI / AI Agents
```

### Engineering Approach

The projects focus on building **reusable, scalable and production-oriented data pipelines**, rather than simply writing SQL transformations.

Key principles:

`Automation → Reusability → Scalability → Data Quality → Performance → Maintainability`
---

## 📈 What I'm Currently Building

- Advanced Snowflake + dbt projects
- Metadata-driven ETL frameworks
- Snowflake AI/Cortex use cases
- Data quality & observability solutions
- Production-style data engineering projects

---

## 📚 Core Expertise

```text
SQL                 ████████████████████
Snowflake           ████████████████████
ETL / ELT           ███████████████████
dbt                 ███████████████
Informatica IICS    ███████████████████
Data Architecture   ██████████████
Python              ████████████
AWS S3              █████████████
```

---

## 🎯 Career Objective

I am focused on building expertise in **modern cloud data engineering and Snowflake architecture**, with the goal of taking ownership of complex data platforms and delivering measurable business impact.

---

## 🤝 Let's Connect

- 💼 LinkedIn: [Shubham Garje](https://www.linkedin.com/in/shubh-garje/)
- 🐙 GitHub: You're already here 😄

> **Build. Automate. Optimize. Repeat.**
