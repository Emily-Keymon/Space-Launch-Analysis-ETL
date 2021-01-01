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
1.  Imported PyMongo.
2.  Initialized PyMongo to work with MongoDB.
3.  Declared the database:  spacex_db.
4.  Declared the collection:  db.news.
5.  Added dataframe to database.
6.  Converted to dictionary.

---
## Results
![MongoDB_screenshot](https://user-images.githubusercontent.com/64673015/103444684-65809980-4c30-11eb-8638-140d2b231abf.PNG)

