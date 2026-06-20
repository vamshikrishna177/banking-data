# Real-Time ETL Pipeline using Databricks Medallion Architecture

## Project Overview

This project demonstrates the design and implementation of an end-to-end ETL pipeline using Databricks and PostgreSQL following the Medallion Architecture (Bronze, Silver, and Gold layers).

The objective was to address a common business challenge where analytical reports were generated from stale or inconsistent data. The solution enables source system updates from PostgreSQL to be reflected automatically in Databricks, ensuring that business users have access to accurate and up-to-date information for reporting and decision-making.

## Business Problem

Organizations often struggle with maintaining reliable reporting datasets when source systems are updated frequently. Manual data refreshes, inconsistent transformations, and lack of monitoring can lead to reporting delays and data quality issues.

This project solves these challenges by:

* Automating data ingestion from PostgreSQL.
* Maintaining raw and historical data for traceability.
* Applying standardized transformation logic.
* Delivering curated business-ready datasets.
* Providing automated monitoring and notification mechanisms.

## Solution Architecture

PostgreSQL (Source System)

↓

Bronze Layer (Raw Data + Metadata)

↓

Silver Layer (Data Cleansing & Transformations)

↓

Gold Layer (Business Ready Datasets)

↓

Reporting & Genie Analytics

## Key Features

### Data Ingestion

* Ingested data from PostgreSQL into Databricks.
* Captured source updates to keep analytical datasets synchronized.

### Bronze Layer

* Stored raw source data.
* Created metadata tables to track ingestion and processing activities.
* Preserved source records for auditability and troubleshooting.

### Silver Layer

* Applied data cleansing and transformation logic.
* Standardized and validated incoming records.
* Prepared datasets for downstream consumption.

### Gold Layer

* Created business-ready tables optimized for reporting and analytics.
* Delivered curated datasets for end-user consumption.

### Workflow Automation

* Automated the complete ETL workflow using Databricks Jobs.
* Scheduled pipeline execution without manual intervention.

### Monitoring & Alerting

* Configured email notifications for successful and failed job executions.
* Improved operational visibility and faster issue identification.

### Analytics Enablement

* Published Gold layer datasets for reporting.
* Integrated Databricks Genie to support natural language queries and self-service analytics.

## Technologies Used

* Databricks
* PySpark
* Delta Lake
* PostgreSQL
* Databricks Workflows / Jobs
* SQL
* Databricks Genie

## Outcome

The solution provides a scalable and automated ETL framework that transforms operational data into trusted analytical datasets. By implementing Medallion Architecture, automated workflows, and monitoring capabilities, the project demonstrates modern data engineering practices for reliable reporting and business intelligence.
