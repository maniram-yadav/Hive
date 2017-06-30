## DDL Queries

  DDL stands for Data Definition Language. It is all about defing the tbale columns , their relation and key constraints based on which data of two table can be related to each other. DDL queries basically include *creating table , altering table, defining key constraints , deletion of table any many more other.*
  
 **Table creation**

Following query format is used for creating table 

```
CREATE [TEMPORARY] [EXTERNAL] TABLE [IF NOT EXISTS] [db_name.] table_name

[(col_name data_type [COMMENT col_comment], ...)]
[COMMENT table_comment]
[ROW FORMAT row_format]
[STORED AS file_format]

```
* Example : *
![Create tables](https://github.com/maniram-yadav/Hive/blob/master/images/createtable.png)

We can be export any file which stores some data to the database table. But condtion is that the file should have a standard format of text.
In above given figure the table contain four fields and query part *ROW FORMAT DELIMITED* will be used when we are going to load any text file to the database in which each and every field will be seperated by comma and row will be terminate by *\n*(new line). One row of the text file will be stored in on tuple of the database schema.

#### ALTER TABLE
 alter command is used for making modification in the table definition.By using alter command we can change the row definition , table name , relation between table etc.
 Let us see example one by one ...
 
 add.
#####  Adding new column
Query Format:
```
 alter table <table name> add columns (<new column name> <type>)
```

** Example **
![Add column](https://github.com/maniram-yadav/Hive/blob/master/images/addcolumn.png)

> In above example new column eaddress has been added to the schema.


#####  Change column definition
  Query Format :
   ```
   alter table <table name> change <old column name> <new column name> <type> ;
   ```
   ** Example **
   ![change column name](https://github.com/maniram-yadav/Hive/blob/master/images/changecolumn.png)
   > In above example column name has been change from eaddress to eadd.
   
   
#####  Replace column :
   ```
   alter table <table name> replace columns (column specifications) ;
   ```
   ** Example **
   ![Replace column](https://github.com/maniram-yadav/Hive/blob/master/images/replacecolumns.png)
   > In above example all the column of the table has been replaced by two new column.
   
   ##### Rename Table
   ```
   alter table <table name> rename <old table name> to <new name> ;
   ```
   ** Example **
   ![Rename table](https://github.com/maniram-yadav/Hive/blob/master/images/altertable.png)
   > In above example all the column of the table has been replaced by two new column.
   
   
   
   
