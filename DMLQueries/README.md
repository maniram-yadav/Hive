## [:arrow_left:Previous](https://github.com/maniram-yadav/Hive/tree/master/DDLQueries) :point_left:


_____________________________ :door: [Home](https://github.com/maniram-yadav/Hive) :door: _____________________________

### DML (Data Manipulation Language) Queries

  DML stands for Data Manipulation Language. It is used to retrieve, store, modify, delete, insert 
  and update data in database.   Examples: SELECT, UPDATE, INSERT statements.
  
  #### Data Insertion 
  
 In case of hive we mostly use to insert data from the file. The file may be text file ,
 sql file , json file or any other which is supported by the database. The data stored in 
the file follow a special rule based on which table is defined. You can learn from  the
previous tutorial. We can load the data from the local disk or from the HDFS file. All the
data from the file is stored in database trable.
     
We use the following query format to load the data from file in the database :point_down:
    
 ```
    load data local inpath <your file path> overwrite into table <database table name>;
 ```
**Example**:point_down:
    ![load data](https://github.com/maniram-yadav/Hive/blob/master/images/loaddata.png)
    
> In the above given example we have loaded data from local disk of computer. After loading
data is stored in the database table.
    
##### select queries
select queries is used for fetching data from the database.
we use the following format for selecting data from database.
      
 ```
      select * from <database table name>;
 ```
**Example**:point_down:
      ![select from database](https://github.com/maniram-yadav/Hive/blob/master/images/selectdata.png)
      
The **_*_** symbol in above query has been used for fetching data from all the columns.
If you want to specify column name of table from which only data will be shown.
The the column names of the table can be at the place of * in the queries.
Query Format :

```
      select <column1>,<column 2>,..., <column n> from  <table name>; 
```

**Example**:point_down:
      ![select column](https://github.com/maniram-yadav/Hive/blob/master/images/selectcolumn.png)

we can also select only some of the row based on the some condition by using where clause.

Query Format :
```  
      select * from <table name> where <condition>;
```
**Example**:point_down:
    ![select where](https://github.com/maniram-yadav/Hive/blob/master/images/selectwhere.png)
    
If we want to fetch data in a special order of column value. The we can use order by query.

```
    select * from <table name> order by <column list>

```
    
  
  **Example**:point_down:
    ![order by](https://github.com/maniram-yadav/Hive/blob/master/images/selectorderby.png)
    
    
  
  Another term GROUP BY clause is used to group all the records in a result set using a particular 
    collection column. It is used to query a group of records.
    Query Format :
  
  ```
    select * from <table name> group by <column list>
  
  ```
 **Example**:point_down:
 ![groyp by](https://github.com/maniram-yadav/Hive/blob/master/images/selectgroupby.png)

## [:arrow_left:Previous](https://github.com/maniram-yadav/Hive/tree/master/DDLQueries) :point_left:
