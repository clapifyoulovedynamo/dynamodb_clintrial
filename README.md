# DynamoDB for Clinical Trials

### Needed: AWS Account and credentials, Jupyter Notebook access
### Contains various other iPynb models

The purpose of this notebook is to demonstrate the value of schema-less NoSQL databases as a use case for clinical trial data domains. 
Clinical trial domains very often are customized to the study with a core base of similar variables, thus making them not suitable for traditional relational databases. 
In this use case, ADaM data is being simulated and read-in to DynamoDB using the Primary Key of domain, and the Sort Key of studyid_usubjid. 

This is valuable for getting multiple data domains stored in the same table without having to enforce a standard schema on a SQL table.

As long as the primary key and sort key are present and unique, any and all data can be inserted into an item (row) as attributes. So it doesn't matter if one row of your data has 25 columns and the next row has 50. 

This non-relational approach has manifold benefits for stacking clinical data domains that may not fit exactly into a relational database. 



![Alt Text](https://i.imgur.com/KSAYqOg.gif)
