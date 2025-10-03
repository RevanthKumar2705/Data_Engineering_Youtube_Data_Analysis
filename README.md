YouTube Data Engineering Analysis Project — Inspired by Revanth Kumar
Overview

This project focuses on securely managing, streamlining, and analyzing structured and semi-structured YouTube video data, categorized by video types and trending metrics. The primary goal is to design a robust cloud-based data pipeline for analytics and reporting.

Project Objectives

Data Ingestion: Develop a process to collect and import data from multiple sources.

ETL System: Transform raw, unprocessed data into a clean and structured format suitable for analysis.

Data Lake: Establish a centralized repository to store data from various sources in one place.

Scalability: Ensure the system can efficiently handle increasing data volumes over time.

Cloud Integration: Utilize cloud infrastructure (AWS) to process and manage large datasets that exceed local computing capacity.

Reporting: Build an interactive dashboard to visualize insights and answer key analytical questions.

AWS Services Utilized

Amazon S3: Scalable and secure object storage for maintaining raw and processed data.

AWS IAM: Identity and Access Management for controlling secure access to AWS services and resources.

Amazon QuickSight: A serverless BI and visualization tool for creating dashboards and analytics reports.

AWS Glue: A serverless ETL service for data discovery, preparation, and integration across analytics workflows.

AWS Lambda: A serverless compute service for executing code in response to data events without managing servers.

Amazon Athena: An interactive query service that allows direct querying of data stored in S3 without the need for loading it into a database.

Dataset Description

The dataset, sourced from Kaggle
, provides daily statistics on trending YouTube videos across multiple regions. Each regional dataset includes information such as video title, channel name, publish time, tags, views, likes, dislikes, description, and comment count. A region-specific category_id field is also included via a linked JSON file.

Architecture
<img src="flowchart.jpeg"> The architecture illustrates the end-to-end flow of data ingestion, transformation, storage, and reporting using AWS services.