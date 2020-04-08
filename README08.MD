# Read08

 ## 1.Database Manipulation:

 - CREATE DATABASE database_name	 .... Create a database	
-  DROP DATABASE database_name	      Delete a database	

## 2.Table Manipulation

- CREATE TABLE "table_name"
("column_1" "data_type_for_column_1",
"column_2" "data_type_for_column_2",
... )

- ALTER TABLE table_name ADD column_name datatype......Add columns in an existing table.

- ALTER TABLE table_name DROP column_name datatype...... Delete columns in an existing table.

- DROP TABLE table_name........Delete a table.


## 3.Index Manipulation

- INSERT INTO table_name
VALUES (value_1, value_2,....)	                       Insert new rows into a table.

- INSERT INTO table_name (column1, column2,...)
VALUES (value_1, value_2,....)

- UPDATE table_name
SET column_name_1 = new_value_1, column_name_2 = new_value_2
WHERE column_name = some_value	                                             Update one or several columns in rows.

- DELETE FROM table_name
WHERE column_name = some_value	                                Delete rows in a table.


- TRUNCATE TABLE table_name	      Deletes the data inside the table.