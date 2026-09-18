# Swiggy_Food_Delivery_Analytics-Microsoft_Fabric_PowerBI

## Swiggy Food Delivery Analytics

An end-to-end data analytics project built using Microsoft Fabric and Power BI to analyze food delivery operations, customer behavior, restaurant performance, orders, revenue, and delivery metrics.

The project demonstrates how raw business data can be ingested into a Fabric Lakehouse, transformed and cleaned, loaded into a Data Warehouse, modeled into a semantic layer, and finally visualized through an interactive Power BI report.

### 📌 Project Overview

Swiggy generates a large amount of data from food orders, customers, restaurants, locations, dishes, and delivery operations.

The goal of this project is to build a complete analytics solution that converts raw Swiggy data into structured and business-ready data for reporting and analysis.

The project follows an end-to-end flow:

### Raw Files → Lakehouse → Data Transformation → Lakehouse Tables → Data Warehouse → Semantic Model → Power BI Report

## 🎯 Project Objectives

The main objectives of this project are:

- Store raw Swiggy datasets in a Fabric Lakehouse.
- Clean and transform the raw data.
- Validate data quality before loading it into the warehouse.
- Store business-ready data in a Data Warehouse.
- Build a structured data model for analytics.
- Create a Power BI Semantic Model using Direct Lake.
- Develop an interactive Swiggy Analytics report.
- Publish the final report and semantic model to the Fabric workspace.
- Provide useful insights into orders, revenue, restaurants, locations, and delivery performance.

## 1. Fabric Workspace

The project started by creating a dedicated Microsoft Fabric workspace.

The workspace contains the main components used throughout the project:

Lakehouse
Data Warehouse
Data Pipeline
Power BI Semantic Model
Power BI Report

This provides a single environment to manage the complete analytics solution.

## 2. Data Ingestion into Lakehouse

The first stage was to load the raw Swiggy datasets into the Fabric Lakehouse.

The raw files were stored in the Lakehouse under the Files section.

The Lakehouse was used as the initial storage layer for the raw source data.

At this stage, the data was kept in its original/raw form before applying transformations.

## 3. Data Cleaning and Transformation

After ingesting the raw data, the next step was to prepare the data for analytics.

The raw datasets were cleaned and transformed before being used for reporting.

Some of the data preparation activities included:

Correcting data types.
Handling incorrect or inconsistent values.
Standardizing data.
Preparing date fields.
Validating order-related values.
Removing or handling invalid records.
Preparing the datasets for analytical modeling.
Checking relationships between related datasets.

The purpose of this stage was to make sure that the data loaded into the analytical tables was clean and usable.

## 4. Loading Clean Data into Lakehouse Tables

After the transformation process, the cleaned datasets were loaded into the Tables section of the Fabric Lakehouse.

The Lakehouse therefore contains business-ready tables rather than only the original raw files.

## 5. Data Pipeline

Once the cleaned Lakehouse tables were ready, a Microsoft Fabric Data Pipeline was created.

The pipeline was used to move the prepared data from the Lakehouse into the Data Warehouse.

## 6. Data Warehouse

The cleaned data was loaded into a Fabric Data Warehouse.

The warehouse was designed using a Star Schema to support analytical reporting.

## 7. Data Validation in Warehouse

After loading the data into the warehouse, the warehouse tables were validated to make sure the data was correctly loaded.

Validation included checking things such as:

### Record validation
Checking whether the expected records were successfully loaded from the Lakehouse into the Warehouse.

### Referential integrity
Checking relationships between fact and dimension data.

## 8. Power BI Semantic Model

After validating the warehouse data, a Power BI Semantic Model was created on top of the warehouse.

The model was configured using Direct Lake.

The semantic model provides the business layer between the warehouse and the Power BI report.

It contains:

- Tables
- Relationships
- Measures
- KPIs
- Business calculations

The model follows the warehouse's analytical structure so that Power BI can efficiently consume the data.

## 9. Measures and KPIs

Some of the key business measures created for the project include:

Total Orders: Measures the total number of orders.
Total Revenue: Measures the total revenue generated from orders.
Average Order Value: Measures the average revenue generated per order.

## 10. Power BI Report

After creating and validating the semantic model, a Swiggy Analytics Power BI report was created.

Instead of connecting the report directly to the raw data, the report connects to the already published Power BI Semantic Model in Microsoft Fabric.

## 11. Publishing to Fabric

Once the Power BI report was completed, it was published to the Microsoft Fabric workspace.
