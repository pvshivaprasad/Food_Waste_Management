# Food Waste Management System

A data-driven food waste management platform that connects food providers with receivers while providing tools to manage listings, claims, and food distribution data.

The application combines **Python, Streamlit, SQLite, SQL, and Pandas** to provide an interactive system for managing surplus food and analyzing food wastage patterns.

<p align="center">
  <a href="https://foodwastemanagement814.streamlit.app/">
    <img src="https://img.shields.io/badge/Live_Demo-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" alt="Live Demo"/>
  </a>
  <a href="https://github.com/pvshivaprasad/Food_Waste_Management">
    <img src="https://img.shields.io/badge/Source_Code-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
  </a>
</p>

---

## Overview

Food wastage is a significant problem while many organizations and communities continue to face food shortages.

This project provides a centralized system where food availability, providers, receivers, and claims can be managed and analyzed efficiently.

The application works with structured food distribution data and provides an interactive Streamlit interface backed by a SQLite database.

The project was originally developed as part of a **Labmentix internship project** and was later organized as a deployable web application.

---

## Features

- Manage food providers and receivers
- Maintain available food listings
- Track food claims and their status
- Perform CRUD operations through the application
- Store structured data using SQLite
- Import and process CSV datasets using Pandas
- Analyze food availability across locations
- Identify active providers and receivers
- Analyze food and meal type distributions
- Track claim status and food distribution activity
- Execute SQL-based analytical queries
- Explore results through an interactive Streamlit interface

---

## Tech Stack

| Technology | Usage |
|---|---|
| Python | Core application logic and data processing |
| Streamlit | Interactive web application |
| SQLite | Relational data storage |
| SQL | Data querying and analysis |
| Pandas | Data cleaning and transformation |
| Jupyter Notebook | Exploratory analysis and development |

---

## System Workflow

```text
CSV Datasets
     │
     ▼
Data Processing
   (Pandas)
     │
     ▼
SQLite Database
     │
     ├── Providers
     ├── Receivers
     ├── Food Listings
     └── Claims
     │
     ▼
SQL Queries & Analysis
     │
     ▼
Streamlit Application
     │
     ▼
Interactive Data Exploration
```

---

## Dataset

The system works with four primary datasets.

### Providers

Contains information about organizations or individuals providing surplus food.

### Receivers

Contains information about organizations or groups receiving available food.

### Food Listings

Stores details about available food, including food type, quantity, location, and meal information.

### Claims

Tracks claims made against available food listings and their corresponding status.

---

## Analysis & Insights

The application supports several analytical views, including:

- Provider distribution across cities
- Receiver distribution across cities
- Most active food providers
- Most active receivers
- Available food quantities
- Food type distribution
- Meal type analysis
- Claim status distribution
- Food listing and claim relationships
- Location-based food availability

SQL queries are used alongside Pandas processing to extract useful information from the underlying data.

---

## Database Design

The application uses a relational SQLite database containing the major entities:

```text
Providers
    │
    └──── Food Listings
              │
              └──── Claims
                      │
                      └──── Receivers
```

The database schema is available in:

```text
schema.sql
```

---

## Project Structure

```text
Food_Waste_Management/
│
├── .streamlit/
│
├── app.py
│
├── Labmentix_Food_Wastage_System_with_Streamlit.ipynb
│
├── schema.sql
├── food.db
│
├── providers_data.csv
├── receivers_data.csv
├── food_listings_data.csv
├── claims_data.csv
│
├── requirements.txt
├── .gitattributes
└── README.md
```

---

## Getting Started

### Prerequisites

Make sure Python 3 is installed.

Check your installation:

```bash
python --version
```

### Clone the Repository

```bash
git clone https://github.com/pvshivaprasad/Food_Waste_Management.git
cd Food_Waste_Management
```

### Create a Virtual Environment

Windows:

```bash
python -m venv venv
venv\Scripts\activate
```

macOS/Linux:

```bash
python3 -m venv venv
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run the Application

```bash
streamlit run app.py
```

The application will normally be available at:

```text
http://localhost:8501
```

---

## Live Application

The deployed application can be accessed here:

**https://foodwastemanagement814.streamlit.app/**

---

## Future Improvements

Potential improvements include:

- User authentication and role-based access
- Automated expiry notifications
- Geographic matching between providers and receivers
- Improved analytics dashboards
- Food demand forecasting
- Recommendation-based provider-receiver matching
- Cloud-hosted database integration
- Automated reporting

---

## Author

**Venkata Shiva Prasad Punna**

Computer Science (AI & ML)  
Python • AI/ML • Backend Development

[GitHub](https://github.com/pvshivaprasad)
