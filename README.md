Streaming Data Insights with Kafka and Hadoop
Overview
This project aims to analyze streaming data from the Amazon Metadata dataset using Apache Kafka for real-time data processing and Hadoop for distributed data analysis. By leveraging Kafka's fault-tolerant, scalable streaming capabilities and Hadoop's distributed processing power, we can efficiently process and analyze large volumes of data in real-time.

Approach
Preprocessing:
The dataset is initially sampled to ensure manageability, and then preprocessed to clean and format it for analysis.
Preprocessing steps include removing unnecessary fields, cleaning text data, converting data types, normalizing data, and handling missing values.
Streaming Pipeline Setup:
Kafka is used to set up a streaming pipeline with a producer application to stream preprocessed data and three consumer applications to subscribe to the data stream.
Frequent Itemset Mining:
Two consumers implement the Apriori and PCY algorithms for frequent itemset mining, providing real-time insights and associations.
The third consumer is used for innovative analysis, employing techniques suitable for streaming data such as sliding window approach, approximation techniques, or online algorithms.
Database Integration:
MongoDB is chosen for database integration due to its NoSQL nature, which fits perfectly for handling unstructured data like JSON.
Each consumer is modified to connect to MongoDB and store the results in separate collections.
Bash Script for Project Execution:
A bash script is provided to automate the setup and execution of the project, including starting Hadoop services, Zookeeper, Kafka server, initializing Kafka topics, and running the producer and consumers.
Why Kafka and Hadoop?
Kafka provides fault-tolerant, scalable streaming capabilities, allowing us to handle high-throughput data streams efficiently.
Hadoop's distributed processing capabilities enable us to analyze large volumes of data in parallel, making it suitable for processing and mining streaming data from the Amazon Metadata dataset.
