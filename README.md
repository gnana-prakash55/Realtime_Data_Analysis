# Realtime_Data_Analysis
It is a Realtime Data Analysis Project using some tools are Apache Kafka,Apache Hadoop,Apache Spark,Apache Cassandra,Apache Superset and MySQL

I used Jupyter notebook as Pyspark shell.You can copy and paste the below line in your bashrc file.
 >   export PYSPARK_DRIVER_PYTHON=jupyter
 
 >   export PYSPARK_DRIVER_PYTHON_OPTS='notebook'
    
You can use this command to open Jupyter notebook as Pyspark Shell.

'pyspark --packages com.datastax.spark:spark-cassandra-connector_2.12:3.0.0,mysql:mysql-connector-java:8.0.22,org.apache.spark:spark-sql-kafka-0-10_2.12:3.0.1'

The above command will download the libraries required.

## Apache Kafka
It is one of the popular distributed messaging platform which is used to stream data.I have used this tool to stream the orders.csv inside data folder.In this project, I have simulated that the orders are coming from the e-commerce website.But it comes from our orders.csv inside the data folder as a stream from kafka topic.

## Apache Hadoop
It is a popular framework for distributed storage.In tis project,I used HDFS to store the customers data(inside data folder).Using Customers data we can get some insights from the data.

## Apache Spark
It is one of the most popular distributed processing engine.I used Spark Structured Streaming to process the realtime data and store it in the Apache Cassandra(raw data) and MySQL(processed data for analysis).

## Apache Cassandra
It is one of the popular NoSQL database and I used it to store the Streaming raw data.

## MySQl
To store the processed and aggregated data for analysis, I used MySQL.

## Apache Superset
It is one of the most popular datavisualisation tool.I have connected MySQL and Superset for analysis.You can check[https://superset.apache.org/docs/databases/mysql] to connect Superset and MySQL.

