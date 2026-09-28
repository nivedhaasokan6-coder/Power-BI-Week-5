# WEEK 5 – POWER BI HEALTHCARE DATA ANALYSIS

## Project Overview

This project focuses on cleaning, transforming, and organizing a healthcare dataset using **Power BI Desktop and Power Query Editor**. The dataset contains patient details, medical conditions, admission information, hospital details, insurance providers, billing amounts, medications, and test results. 

The data was cleaned and transformed to create three main tables: **Dim_Patient, Dim_Admission, and Billing**. Patient ID and Admission ID were created to organize the data and connect the tables.

## Objectives

The main objectives of this project are to clean the healthcare dataset, standardize the data, create age groups, separate patient and admission information, create the Billing table, and build a structured data model in Power BI.

## Tools and Technologies

* Power BI Desktop
* Power Query Editor
* Healthcare Dataset
* Power BI Data Model

## Project Process

The healthcare dataset was first imported into Power BI and opened in Power Query Editor. The categorical columns were cleaned using **Trim** and **Clean**, and the Name column was standardized using **Capitalize Each Word**. An Age Group column was then created with the groups **0-18, 19-35, 36-60, and 60+**. 

The original dataset was duplicated to create **Dim_Patient**, where patient-related columns were retained and a **Patient ID** was created using an Index Column. Another duplicate was used to create **Dim_Admission**, where admission-related columns were retained and an **Admission ID** was created. 

A **Billing** table was then prepared with the required patient, admission, and billing information. It was merged with Dim_Patient to obtain Patient ID and then merged with Dim_Admission to obtain Admission ID. Both merges used a **Left Outer** join. 

##  Final Result

The final Power BI model contains **Dim_Patient, Dim_Admission, and Billing**. The Billing table contains the required billing information along with Patient ID and Admission ID. These tables provide a structured format for further healthcare data analysis and visualization. 


Available next action: Create a downloadable DOCX file here in this chat containing the editable prose above
