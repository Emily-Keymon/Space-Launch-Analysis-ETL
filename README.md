# Space Launch Analysis: ETL - Extract, Transform, Load
The goal of this project was to extract, transform and load data to ensure the media coverage for Space X launches was effective.  

---
## Data Sources
* Next Space Flight:  https://nextspaceflight.com
* HuffPost:  https://www.huffpost.com/

---
## Tools Used
* PyCharm - Python IDE
* Jupyter Notebook
* Python - Pandas, NumPy, Datetime, PyMongo
* MongoDB Compass - MongoDB IDE

---
## Tasks
### Data Source 1:
### Extract
1.  Imported the Space X launch data CSV file as Pandas data frame.

### Transform
1.  Removed extra columns.
2.  Created dataframe for SpaceX data.
3.  Saved new dataframe as csv file.  

### Data Source 2:
### Extract
1.  Imported the HuffPost news data JSON file as Pandas data frame.

### Transform
1.  Removed extra columns.
2.  Created dataframe for SpaceX data.
3.  Saved new dataframe as csv file.
4.  Merged both launch and news dataframes.

## Load
1.  

The last step was to transfer our final output into a database. We created a database and respective table to match the columns from the final Panda's Data Frame using MongoDB.  We chose this non-relational database because it proves to be ideal for storing data that may be changed frequently. 
* PyMongo was used to work with MongoDB
* PyMongo.MongoClient was used to establish the connection
* client.db was used to declare the database
* db.collection.insert_many was used to add the data frame to the database
* df.to_dict was used to convert the records to dictionary for storage in the database

---
## Results

### Final Tables
* Company Name
* Location
* Date
* Detail
* Status Rocket
* Rocket
* Status Mission
* Category
* Headline
* Authors
* Link
* Short Description


