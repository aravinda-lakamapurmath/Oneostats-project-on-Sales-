# Sales Data Processing Pipeline

This repository contains the setup and configuration scripts for a Sales Data Processing Pipeline using Azure services. The pipeline ingests raw sales data, processes it, and visualizes it using Power BI.

## Repository Structure

- **`azure-cli/`**: Contains scripts for setting up Azure Data Lake Storage (ADLS).
  - `setup_adls.sh`: Azure CLI script for creating storage accounts and containers.

- **`adf-pipeline/`**: Contains scripts and templates for setting up Azure Data Factory (ADF) pipelines.
  - `create_adf_pipeline.py`: Python script for creating and managing ADF pipelines.
  - `adf_pipeline_template.json`: JSON template for the ADF pipeline configuration.

- **`sql-scripts/`**: Contains SQL scripts for transforming and processing sales data.
  - `transform_sales_data.sql`: SQL script for creating tables and transforming sales data.

- **`powerbi/`**: Contains documentation for connecting and visualizing data with Power BI.
  - `PowerBI_Connection_Guide.md`: Guide for connecting Power BI to Azure SQL Database and creating visualizations.

## Setup Instructions

### 1. **Azure Data Lake Storage (ADLS) Setup**

Run the `setup_adls.sh` script to create the necessary ADLS containers:

```bash
cd azure-cli
bash setup_adls.sh
