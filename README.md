# Google Business Certification (GBC) Student Enrollment Data

## Overview
This repository contains the raw enrollment dataset for students participating in the **Google Business Certification (GBC)** program across multiple batches and locations in India during 2023. The data was collected by training partners and includes demographic, academic, geographic, financial, and participation information for each enrolled student.

The dataset is provided as a single Excel file: **`Student Data.xlsx`**.

## Dataset Contents
The Excel file contains **198 records** (student entries) with the following key fields:

### **Core Identification & Program Info**
- **Batch code**: Unique identifier for each training batch (e.g., ANP-C4782, ANP-C5232).
- **Student name**: Full name of the enrolled student.
- **Date of Birth**: Student’s date of birth (YYYY-MM-DD format).
- **Online Registration ID**: Unique ID assigned during online registration.
- **Center code & Name**: Code and name of the training center (e.g., ASGGL - Guwahati, JHGGL - LALPUR (M/S RIIT), TSGGL - HYDERABAD(Dilsukh Nagar), TNGGL - TAMBARAM).
- **Student code**: Internal student identifier used by the program.
- **Program Name**: "Google"
- **Course**: "GBC" (Google Business Certification)
- **Funder**: "Google" (All students are fully funded by Google; no fees charged to students).

### **Batch & Delivery Details**
- **Batch start date & End date**: Planned duration of the course.
- **Batch actual end date**: When the batch actually concluded (if completed).
- **Mode of Delivery**: How the course was delivered:
    - Online (Blended)
    - Offline (Blended)
    - Hybrid (Blended)
    - App based Attendance Process
    - Manual Attendance (Special Case)
    - Partner center where Biometric is not allowed
- **Batch Type**: Specific operational model of the batch (e.g., "Online mode", "App based Attendance Process").
- **Base assessment required**: Indicates if a foundational assessment was required (All = "No").
- **Base marks / Base date**: Score and date of the initial assessment (where recorded).
- **Mid marks / Mid date**: Score and date of mid-course assessment (for some batches).
- **Final marks / Final Date**: Score and date of the final assessment (for completed batches).
- **Final assessment mode**: How the final assessment was conducted ("Internal" or "External").
- **Partner Status**: Information about the training partner's status.
- **Batch Status**: Current status of the batch ("Running" or "Ended").

### **Student Demographics & Profile**
- **Gender**: Male or Female.
- **Qualification**: Educational background (e.g., Graduate, 12th Pass, Post Graduate, Under Graduate Diploma).
- **Completed ITI course**: Marked as "N/A" for all students.
- **No Of Family Members**: Number of members in the student's household (range: 2–9; one record shows an implausible value: 2,147,483,647).
- **Economic Status**: APL (Above Poverty Line) or BPL (Below Poverty Line).
- **Category**: Social category (General, OBC, SC, ST).
- **Admission Date**: Date when the student was formally admitted into the batch.

### **Location & Contact**
- **District**: District where the training center is located (e.g., Kamrup, Ranchi, Rangareddy, Chengalpattu).
- **State**: State where the training center is located (Assam, Jharkhand, Telangana, Tamil Nadu).
- **Actual Center Code**: Confirms the physical location of the center (matches Center code).
- **Mobile No**: Student’s mobile phone number.
- **Email Id**: Student’s email address (note: some contain typos like `gamil.com`, `gmil.com`).

### **Administrative & Management**
- **Trainer Name**: Name(s) of the trainer(s) assigned to the batch.
- **Enrollment Status**: All students are marked as "enrolled".
- **Re-instate Status**: All students are marked as "Enrolled".
- **RM Emp. Code & RM Name**: Employee ID and name of the Relationship Manager overseeing the batch.
- **Blended status**: Indicates if blended learning was used ("Yes" or "No").

### **Participation Status**
- **Status**: Critical field indicating actual participation:
    - **Joined**: Student actively participated in the program.
    - **Not Joined**: Student enrolled but did not attend or participate.

> ⚠️ **Important Note**: A significant portion of students (approximately 25%) have a status of "**Not Joined**", despite being enrolled. This highlights a notable attrition rate between enrollment and active participation.

## Key Observations from the Data
- **Geographic Spread**: Students are enrolled from four Indian states: Assam, Jharkhand, Telangana, and Tamil Nadu.
- **Funding Model**: **Zero cost to students** — Course Fees, Fees Paid, and Fees Due are all ₹0 for every record. The program is fully sponsored by Google.
- **Gender Distribution**: Majority of students are female (~65%).
- **Education Level**: Most students hold a Graduate degree; a large number (especially in Telangana and Tamil Nadu) are 12th Pass.
- **Performance Variation**: Final and base assessment scores show a wide range—from very low (0–20) to very high (80–100)—suggesting varied prior knowledge or engagement levels.
- **High Attrition**: Many students who enrolled ("enrolled") did not join ("Not Joined"), regardless of location or delivery mode.
- **Data Quality Notes**:
    - Some email addresses contain typos (e.g., `gamil.com` instead of `gmail.com`).
    - Several cells (especially for Mid/Final marks) are empty (`| |`) for ongoing or incomplete batches.
    - One record has an implausibly high value for “No Of Family Members” (2,147,483,647).

## Purpose of This Repository
This repository serves as a **centralized archive** of the original, unmodified enrollment data. It allows stakeholders (program managers, trainers, partners, auditors) to access, verify, and reference the source data for reporting, auditing, or future analysis.

## How to Use This File
1. Download the `Student Data.xlsx` file from this repository.
2. Open it using Microsoft Excel, Google Sheets, LibreOffice Calc, or any compatible spreadsheet software.
3. Use filters, sorting, and pivot tables to explore the data by:
    - State
    - Batch Code
    - Status (Joined / Not Joined)
    - Qualification
    - Category
    - Gender

## Important Notes
- **No Analysis Provided**: This repository contains only the raw Excel file. No charts, graphs, or summaries are included.
- **Privacy**: All personal data is presented as-is from the source. Ensure compliance with local data privacy regulations when handling this data externally.
- **Updates**: If new data is added or corrections are made, a new version of `Student Data.xlsx` will be uploaded here with a timestamped filename (e.g., `Student Data_2024-06-01.xlsx`).

---

**Last Updated**: [Insert Date You Upload This README]  
**Source**: Google Business Certification Program – Training Partners  
