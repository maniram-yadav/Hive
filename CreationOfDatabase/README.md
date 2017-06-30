
   ### Hive Database Schema Queries
   
   Schema queries are used for knowing all about existing schema in the database like listing schemas , droping etc.
   
   
   **Listing Databases**
   
You have to use below given *Query* for showing databases which has already been created in the database.

```
 show databases;
```
The above given hive query will output something in below given image

![show databases](https://github.com/maniram-yadav/Hive/blob/master/images/showdb.png)

There is no any database except *default* in the database. So we have to create a database *hivedb* for storing the data when will work in hive in some of the next tutorial.

We have to use following query for creating database schema

```
create database <New database name>;
```

Example :
![create database hivedata](https://github.com/maniram-yadav/Hive/blob/master/images/createdb.png)

If you are going to use the query **_show databases_**. The it will list newly created database on the terminal like first image of this page given above.

**Deleing Database**

For deleting any database schema which already exists in the database we need to use query give below .
```
drop database <your existing database name>;
```
Example :
![drop database database name](https://github.com/maniram-yadav/Hive/blob/master/images/sdropdb.png)

Make sure the database schema which you want to delete (drop) have no any table. Otherwise it will give a caution message to you. So firstly delete all the table from the given schema the drop the schema.  :point_right:   **[Read More]()**

## [:arrow_left:Previous]() :point_left: ____________________________ :point_right:        [Next :arrow_right:]()
