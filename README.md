# Snowflake_pipeline_using_Docker_Airflow


![alt text](https://github.com/Chanikya-digumarthi/Snowflake_pipeline_using_Docker-Airflow/blob/main/Architecture.jpg)


## Project Overview
The goal of this project is to create a robust and scalable data pipeline that processes, transforms, and loads data into Snowflake, a cloud-based data warehousing platform. The pipeline will be orchestrated and scheduled using Apache Airflow, and the entire infrastructure will be containerized using Docker for easy deployment and management.

## Infrastructure Setup
Snowflake: Set up a Snowflake account and create the required databases, schemas, and tables to store and process the data.  
Airflow: Install and configure Apache Airflow, a popular open-source workflow scheduler and task management platform. Configure the Airflow web server and scheduler components.  
Docker: Install Docker and set up a Docker environment to containerize the pipeline components.  

## Workflow
Step1:  Create a snowflake database and a schema.  
Step2:  Configure a snowflake connection in Airflow by providing credentials.  
Step3:  Create a DAG file that runs using Airflow and deploy it using docker container

## Airflow working
Airflow runs the DAG defined in the DAG.py file according to the schedule.  
In our case, the DAG defined will create a table in the snowflake database and only runs manually.  
When it runs, using snowflake connection defined, the create table SQL command creates a table with three columns in the database.
As the Airflow is using docker container, the software package can be delpoyed in any environment.

