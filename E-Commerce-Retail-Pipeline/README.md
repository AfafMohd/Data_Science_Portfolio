# E-Commerce Database System with Automated Data Pipeline

A comprehensive database system for an e-commerce platform with automated data validation, continuous integration pipeline and data analysis.

## 🚀 Overview

This project demonstrates full-stack data engineering capabilities by designing and implementing a complete e-commerce database system from scratch. The system features normalized database design, synthetic data generation, automated data validation, and CI/CD pipelines for data management.

## 🛠️ Technical Stack

- **Database**: SQLite with RSQLite
- **Languages**: R, SQL
- **Workflow Automation**: GitHub Actions
- **Data Validation**: Custom validation scripts
- **Reporting**: Quarto for dynamic documentation

## 📊 Key Features

### Database Design
- **8 Normalized Tables** designed to 3NF standards
- **Complex Relationships**: Many-to-many, one-to-many relationships with proper foreign key constraints
- **Derived Columns**: Automated calculation of order totals using SQL views
- **Data Integrity**: Comprehensive primary key and unique constraints

### Data Pipeline
- **Synthetic Data Generation**: Created realistic e-commerce data using `charlatan`, `fakir`, and custom distributions
- **Automated Validation**: Data quality checks for formats, ranges, and business rules
- **CI/CD Integration**: GitHub Actions workflow for continuous data validation and reporting
- **Referential Integrity**: Automated cleanup of orphaned records

### Business Intelligence
- Customer behavior analysis
- Product performance tracking
- Payment method preferences
- Category popularity metrics

## 💡 Technical Highlights

- **Normalized Schema**: Designed entity-relationship diagram with 7 core entities and proper relationships
- **Data Quality Framework**: Implemented 50+ validation rules across all data domains
- **Automated Workflows**: Scheduled data validation and reporting via GitHub Actions
- **Production-Ready**: Handles data updates, integrity checks, and error logging

##  Skills Demonstrated

- Database Design & Normalization
- ETL Pipeline Development
- Data Quality Assurance
- CI/CD for Data Systems
- SQL Optimization
- R Programming for Data Engineering
- Automated Reporting

## 📈 Business Impact

The system enables:
- Real-time data validation for 1,000+ products and customers
- Automated business intelligence reporting
- Scalable data architecture for e-commerce operations
- Continuous data quality monitoring
