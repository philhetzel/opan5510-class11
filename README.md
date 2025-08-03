# SQL for Data Analysis: From Polars to SQL

Welcome to Class 11! In this class, we'll transition from Python Polars to SQL, building on your existing data manipulation knowledge.

## Learning Objectives

By the end of this class, you'll be able to:
1. Write basic SQL queries to retrieve and filter data
2. Perform joins between multiple tables
3. Aggregate data using GROUP BY and aggregate functions
4. Translate common Polars operations to SQL equivalents

## Class Materials

### 1. **class_example.ipynb**
An interactive notebook that covers:
- SQL basics: SELECT, FROM, WHERE
- Joining tables with different join types
- Aggregation with GROUP BY and HAVING
- Comparing SQL syntax to Polars operations

### 2. **lab_example.ipynb**
Practice exercises using the NYC airports dataset to:
- Query flight information
- Join flights with airlines, airports, and planes data
- Analyze flight patterns and performance
- Create complex queries with multiple joins and aggregations

## Dataset Overview

We'll be using the NYC airports dataset containing:
- **nyc_flights.csv**: Flight records with departure/arrival times, delays, etc.
- **nyc_airlines.csv**: Airline information
- **nyc_airports.csv**: Airport locations and details
- **nyc_planes.csv**: Aircraft information
- **nyc_weather.csv**: Weather conditions

## Getting Started

1. Open `class_example.ipynb` to follow along with the lesson
2. Complete the exercises in `lab_example.ipynb`
3. Compare your SQL queries to equivalent Polars operations

## SQL vs Polars Quick Reference

| Operation | Polars | SQL |
|-----------|--------|-----|
| Select columns | `df.select(['col1', 'col2'])` | `SELECT col1, col2 FROM table` |
| Filter rows | `df.filter(pl.col('x') > 5)` | `WHERE x > 5` |
| Group by | `df.group_by('col').agg(...)` | `GROUP BY col` |
| Join | `df1.join(df2, on='key')` | `FROM df1 JOIN df2 ON df1.key = df2.key` |

## Prerequisites

- Understanding of Polars DataFrames
- Basic data manipulation concepts
- Familiarity with relational data concepts

Let's begin your SQL journey!