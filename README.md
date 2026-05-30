# 🚀 Data Modeler – Building a Normalized Star Schema Data Model

## 📌 Project Objective
This project demonstrates the complete process of building a normalized Star Schema in Power BI Desktop, including Power Query data cleaning, relationship creation, hierarchies, and Matrix validation.

## 🛠️ Step 1: Data Import & Cleaning
- Imported all files into Power BI Desktop.
- Opened Power Query Editor.
- Removed blank rows and validated records.
- Applied correct data types.
- Loaded cleaned data into the model.

## ⭐ Step 2: Star Schema Design
### Fact Tables
- Sales_Fact
- Returns_Fact

### Dimension Tables
- Customer_Dim
- Product_Dim
- Region_Dim
- Date_Dim

## 🔗 Relationships Created
- Sales_Fact → Customer_Dim
- Sales_Fact → Product_Dim
- Sales_Fact → Region_Dim
- Sales_Fact → Date_Dim
- Returns_Fact → Sales_Fact
- Returns_Fact → Date_Dim (Inactive)

## 🏗️ Schema Structure
  Customer_Dim
                |
Product_Dim — Sales_Fact — Region_Dim
                |
              Date_Dim
                |
             Returns_Fact

## 📊 Hierarchies
### Date Hierarchy
Year → Quarter → Month → Date

### Region Hierarchy
Country → State → City

### Product Hierarchy
Category → Subcategory → ProductName

## ✅ Matrix Validation
1. Sales by Product Category and Region
2. Return Reasons by Fiscal Year
3. Revenue by Customer Segment

## 🏆 Outcome
Successfully built a scalable Star Schema model with relationships, hierarchies, and Matrix validation in Power BI.

