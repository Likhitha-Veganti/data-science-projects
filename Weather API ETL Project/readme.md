# Weather Data ETL Pipeline with Apache Airflow and AWS

## Overview
This project demonstrates the creation and automation of an Extract, Transform, Load (ETL) pipeline using Apache Airflow. The pipeline extracts current weather data from the OpenWeatherMap API, transforms this data, and loads it into an Amazon S3 bucket. This solution is fully implemented on the AWS cloud platform, showcasing a practical use case of cloud and data engineering tools in tandem to manage and automate data workflows.

## Features
- **Data Extraction**: Utilizes the OpenWeatherMap API to fetch real-time weather data.
- **Data Transformation**: Converts temperature values from Kelvin to Fahrenheit and restructures the data for better usability.
- **Data Loading**: Stores the transformed data into an AWS S3 bucket for further analysis or visualization.

## Prerequisites
Before you begin, ensure you have met the following requirements:
- An AWS account with access to S3 and permissions to create and manage buckets.
- Apache Airflow environment setup either locally or in the cloud (AWS EC2, Google Cloud Composer, etc.).
- Python 3.6 or higher, with `pandas` and `pytz` libraries installed.
- Access to the OpenWeatherMap API (you will need an API key).
