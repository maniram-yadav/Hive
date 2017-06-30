You have to use below given *Query* for showing databases which has already been created in the database.

```
 show databases;
```
The above given hive query will output something in below given image

![show databases](https://github.com/maniram-yadav/Hive/blob/master/images/showdb.png)

There is no any database except *default* in the database. So we create a database *hivedb* for storing the data relating to the hive query.

We have to use following query for creating database schema

```
create database <New database name>;
```

Example :
![create database hivedata](https://github.com/maniram-yadav/Hive/blob/master/images/createdb.png)

If you are going to use the query **_show databases_**. The it will list newly created database on the terminal like above given first image of this page.

**Deleing Database**

For deleting any database schema which already exists in the database we need to use query give below .
```
drop database <your existing database name>;
```
Example :
![drop database database name](https://github.com/maniram-yadav/Hive/blob/master/images/sdropdb.png)

Make sure the database schema which you want to delete (drop) have no any table. Otherwise it will give a caution message to you. So firstly delete all the table from the given schema the drop the schema. **[Read More]()**

## [:arrow_left:Previous]()                                                   ## [Next :arrow_right:]()
