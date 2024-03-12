# YouTube-Data-Harvesting

## Introduction 

* The project described focuses on extracting data from YouTube channels using their channel IDs, processing the extracted data, and storing it in a MongoDB database. Optionally, it provides the functionality to migrate the stored data from MongoDB to MySQL for further analysis. Ultimately, the goal is to analyze the data and provide insights based on customer queries.

## Here's a breakdown of the project phases:
## Data Extraction from YouTube:
* Extracts data from YouTube channels using their channel IDs.
* This likely involves utilizing YouTube Data API to retrieve information such as video details, channel statistics, comments, etc.
## Data Processing:
* Processes the extracted data to organize it into a suitable format for storage and analysis.
* This may involve structuring the data into dictionaries, lists, or DataFrames, handling missing data, cleaning up text fields, and transforming the data as needed.
## Storage in MongoDB:
* Stores the processed data into a MongoDB database.
* MongoDB is a NoSQL database that allows flexible storage of structured and semi-structured data.
## Migration to MySQL:
* Provides the option to migrate the stored data from MongoDB to MySQL.
* MySQL is a relational database management system (RDBMS) that allows for structured storage and querying of data.
## Data Analysis and Insights:
*Analyzes the stored data to derive insights based on customer queries.
*This could involve running SQL queries on the MySQL database, performing data aggregations, calculations, and visualization of results.


* The project demonstrates the versatility of YouTube as a platform for content creation and engagement and highlights the importance of data processing and analysis in deriving meaningful insights from large datasets. It showcases the integration of different technologies and databases to effectively manage and analyze data collected from online platforms like YouTube.


## Required libraries and softwares

### 1. Tools Install

* Virtual code.
* Jupyter notebook.
* Python 3.11.0 or higher.
* MySQL.
* MongoDB.
* Youtube API key.

### 2. Requirement Libraries to Install

* pip install google-api-python-client, pymongo, mysql-connector-python, sqlalchemy, pymysql, pymysql, pandas, numpy, 
  plotly-express, streamlit.
  
 ( pip install google-api-python-client pymongo mysql-connector-python sqlalchemy pymysql pandas numpy plotly-express streamlit )
### NOTE:
* You need to replace with your own youtube API key
* similarly, you need to specify the mongoclient if your are using ATLAS, no need if you are using local
* replace with your own username and password for MYSQL
* You need to run this command inorder to execute the code
  (streamlit run /Users/username/Downloads/youtube_mongo.py)



###  Data Processing

#### Extract data

* Extract the particular youtube channel data by using the youtube channel id, with the help of the youtube API developer console.

#### Process and Transform the data

* After the extraction process, takes the required details from the extraction data and transform it into JSON format.

#### Load  data 

* After the transformation process, the JSON format data is stored in the MongoDB database, also It has the option to migrate the data to MySQL database from the MongoDB database.

### Process and Framework

#### Access MySQL DB 

* Create a connection to the MySQL server and access the specified MySQL DataBase by using pymysql library and access tables.

#### Filter the data

* Filter and process the collected data from the tables depending on the given requirements by using SQL queries and transform the processed data into a DataFrame format.

#### Visualization 

* Finally, create a Dashboard by using Streamlit and give dropdown options on the Dashboard to the user and select a question from that menu to analyse the data and show the output in Dataframe Table and Bar chart.
