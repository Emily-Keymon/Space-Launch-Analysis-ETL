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
2.  Saved new dataframe as csv file.

### Transform
1.  Removed extra columns.
2.  Created dataframe for SpaceX data.

### Data Source 2:
### Extract
1.  Imported the HuffPost news data JSON file as Pandas data frame.
2.  Saved new dataframe as csv file.

### Transform
1.  Removed extra columns.
2.  Created dataframe for SpaceX data.


Data source one was a csv file.  Pandas library was used for transformation.
* pd.read_csv was used to read the file into Jupyter Notebook
* df.drop was used to drop extra columns
* df.value_counts was used to review the amount of data collected
* df.loc was used to filter out SpaceX flights
* df.to_csv was used to save the completed data frame as a csv file


Data source two was a json file.  Pandas library was used for transformation.
* pd.read_json was used to read the file into Jupyter Notebook
* df.str was used to search for SpaceX news
* df.value_counts was used to review the amount of data collected
* df.Index was used to index the data
* df.to_csv was used to save the completed data frame as a csv file
* pd.concat was used to concatenate the two data frames together


## Load
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


