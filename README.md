# Netflix Dataset Cleaning - README

## Overview
This project involves cleaning and preprocessing the Netflix Movies and TV Shows dataset from Kaggle.

## Cleaning Steps

### 1. Missing Values
- Replaced missing `director`, `cast`, and `country` fields with `'Unknown'`
- Filled missing `rating` with `'UNRATED'`
- Filled missing `duration` with `'Unknown'`
- Converted `date_added` to datetime format; invalid entries set to NaT

### 2. Duplicate Removal
- Removed exact duplicate rows

### 3. Standardization
- Stripped and title-cased `country` values
- Converted `rating` values to uppercase
- Renamed all column headers to lowercase with underscores for consistency

### 4. Data Type Fixes
- Ensured proper data types for columns like `release_year` (int), `date_added` (datetime), and `rating` (string)

## Output Files
- `netflix_titles_cleaned.csv`: Cleaned dataset
- `netflix_cleaning_summary.pdf`: Summary of all cleaning steps

## Record Count
- Total records after cleaning: **8807**
