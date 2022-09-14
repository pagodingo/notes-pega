# PRPC Tables *

<<<<<<< HEAD
## Assignment tables

|Name|Description|
=======

## Assignment tables
|||
>>>>>>> bf1bbf3e82fd8997876e586796524da38adf5393
|-|-|
|pc_assign_workbasket| This table holds assignments in work queues and instances of the Assign-Workbasket class.|
|pc_assign_worklist| This table holds assignments on worklists (Assign-Worklist class).|
|pr_assign| This table holds external assignments (Assign-External class), which use the directed web access feature and assignments of all other types. Assignments in the Assign-Corr and Assign-Service classes are also stored as rows in the pr_assign table.|

## Data Object Tables
<<<<<<< HEAD
|Name|Description|
|-|-|
=======

>>>>>>> bf1bbf3e82fd8997876e586796524da38adf5393
|pr_operators| This table contains rows that correspond to instances of the Data-Admin-Operator-ID class.|
|pi_data_connect| This table is associated with the Data-Admin-Connect- class. Instances of the classes derived from this class support service listeners and related interface data.|
|pr_data_admin| This table holds instances of classes derived from the Data-Admin- class, excluding those who are explicitly mapped to other tables.|
|pc_data_uniqueid| This table corresponds to the Data-UniqueID class. It contains a single row for each work item ID format in use. It records the most recently assigned work item ID of that format.|
|pc_data_workattach| Attachments to work items are instances of concrete classes derived from the Data-WorkAttach- class and linked to this table.|
|Pr4_base| This table holds the instances of three foundation classes, Data-Admin-DB-Table ; Data-Admin-DB-Name; Data-Admin-DB-ClassGroup.|
<<<<<<< HEAD
|pr_data_file| Data-Content-Image class is associated with the table.|

## History Tables
|Name|Description|
|-|-|
=======
pr_data_file: Data-Content-Image class is associated with the table.

## History Tables

>>>>>>> bf1bbf3e82fd8997876e586796524da38adf5393
|pc_history_work| This table contains all classes derived from the History-Work- class.|
|pr4_history_rule| This tables contains instances for various rule related works like Restore, Recover, and detailed history|

## Case Tables

<<<<<<< HEAD
|Name|Description|
|-|-|
|pc_work| This table saves the case instances of concrete classes derived from the Work- base class.|

Apart from the ones mentioned above, there are a few other categories of tables to keep in mind.

- **Link Tables** - This type of table stores information about paired object instances. In the Pega Platform database, the names of link tables start with the values pc_link or pr_link.

- **Log table** - This table stores instances of Log- classes.

- **Index Table** - Most Pega Platform DB tables that support indexes have table names that start with pr_index or pc_index and fall under this category.


        Sourced from: https://community.pega.com/blog/four-common-pega-database-tables-you-should-know
=======
|pc_work| This table saves the case instances of concrete classes derived from the Work- base class.|


Apart from the ones mentioned above, there are a few other categories of tables to keep in mind.

- Link Tables: This type of table stores information about paired object instances. In the Pega Platform database, the names of link tables start with the values pc_link or pr_link.

- Log table: This table stores instances of Log- classes.

- Index Table: Most Pega Platform DB tables that support indexes have table names that start with pr_index or pc_index and fall under this category.


Sourced from:
https://community.pega.com/blog/four-common-pega-database-tables-you-should-know
>>>>>>> bf1bbf3e82fd8997876e586796524da38adf5393
