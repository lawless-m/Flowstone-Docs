# PostgreSQL

The best open source database around for SQL.

As well as the native database. also use [[Foreign-Data-Wrappers]] to access other data sources. For instance you can import data from [[Parquet]] files or query [[MySQL]], and even [[ODBC]].

Having said that, it's not perfectly flexible.  Sometimes it won't do cross-database queries. So you have to do the query to a materialized view, and then query it from there. Which is the same as just importing it somehow. 

Some of the great benefits though are stored procedures where you can write functions that the database can call, triggers which is SQL that executes after an update or an insert or delete. 

So for instance, you can have a last-updated field, and then write a trigger that will set that last updated field if any of the other columns are updated. 





