# Live-Weather-Data
Live Weather Data | AWS/Airflow Data Engineering


Goal: Execute an end-to-end ETL pipeline within the AWS ecosystem from data extraction to storage, while also gaining hands-on experience with Apache Airflow by learning and implementing it effectively in the workflow.

Intro

This project explores the power of AWS cloud services to automate the extraction, transformation, and loading of live data. By leveraging a combination of AWS EC2, Ubuntu VM, and Apache Airflow, I crafted a seamless workflow that efficiently handles and processes real-time information. This endeavor highlights the potential of cloud computing in creating dynamic, scalable solutions for data-driven tasks.

Skills

Cloud Infrastructure Management: Setting up and configuring AWS EC2 instances and Ubuntu VMs.

Workflow Automation: Orchestrating ETL processes using Apache Airflow.

API Integration: Extracting real-time data from the OpenWeatherMap API using Python.

Data Transformation: Processing and transforming raw weather data into structured formats.

Data Storage: Efficiently loading and managing transformed data in AWS S3 as CSV files

Tools

AWS EC2: For launching and managing the virtual server environment.

Ubuntu VM: For providing a flexible and secure operating system for development.

Apache Airflow: For orchestrating and automating ETL workflows.

Python: For extracting, transforming, and processing real-time weather data.

OpenWeatherMap API: For retrieving live weather data specific to the city of Chicago.

AWS S3: For scalable and reliable storage of transformed data in CSV format

Code

The entire python code for this project can be found in the Github Repository under weather_dags.py

An Example of what the extracted and transformed data looks like can be found in the Github Repository under current_weather_data_chicago_14082024224104.csv

Step-by-Step Breakdown

Setting up AWS EC2 Instance and Ubuntu VM

The project began by launching an AWS EC2 instance, providing the foundational cloud infrastructure necessary for further development. I selected an appropriate instance type and configured the security settings to ensure a secure environment. Following the instance launch, I set up an Ubuntu virtual machine (VM) on this instance, establishing a flexible and reliable operating system for the project.

Workflow Automation with Apache Airflow

With the VM in place, the next step was to install and configure Apache Airflow. This tool was essential for orchestrating the ETL (Extract, Transform, Load) process, allowing me to schedule and manage workflows efficiently. I connected Airflow to Visual Studio Code (VS Code), enabling seamless development and monitoring of the workflows.

Data Extraction with OpenWeatherMap API

The core of the project involved extracting real-time weather data from the OpenWeatherMap API. I wrote Python scripts that interfaced with the API, focusing on retrieving weather information specific to the city of Chicago. This data extraction process was automated through the Airflow pipeline, ensuring continuous and up-to-date data retrieval.

 Data Transformation with Python

Once the data was extracted, the next phase was to transform it into a structured format suitable for storage and analysis. Using Python, I cleaned and refined the raw weather data, making it more usable for downstream processes. 

Data Storage in AWS S3

After transformation, the processed data was stored in AWS S3 as CSV files. AWS S3 provided a scalable and reliable storage solution, ensuring that the data was securely stored and readily accessible for future analysis. The Airflow pipeline was configured to automatically load the transformed data into the designated S3 bucket.

Apache Airflow Graph

Though this project marked my initial exploration into Apache Airflow, I successfully designed and implemented a functional workflow. Despite its simplicity, the Airflow DAG (Directed Acyclic Graph) effectively managed the ETL process, ensuring that each step from data extraction to storage was automated and seamless. This hands-on experience provided a solid foundation for future, more complex Airflow projects

Summary

This project has greatly advanced my skills in cloud-based data engineering, marking my first successful implementation of an automated ETL pipeline within the AWS environment. The experience allowed me to deeply explore the integration of multiple AWS services, such as EC2, S3, and Apache Airflow. I gained valuable insights into how these tools can be effectively combined to achieve project objectives. This experience has not only enhanced my understanding of AWS but also equipped me with practical knowledge that I can apply to more complex cloud-based projects in the future.
