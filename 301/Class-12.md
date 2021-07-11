# Mongo and Mongoose

## nosql vs sql

- Fill in the chart below with five differences between SQL and NoSQL databases:

|
SQL | NoSQL |
| ------------------------------------------------------- | ----------------------------------------------------- |
| SQL databases are primarily called RDBMS or Relational Databases | NoSQL databases are primarily called as Non-relational or distributed database |
| SQL databases are vertically scalable | NoSQL databases are horizontally scalable |
| Oracle, Postgres, and MS-SQL. | MongoDB, Redis, Neo4j, Cassandra, Hbase. |
| SQL databases are table based databases | NoSQL databases can be document based, key-value pairs, graph databases |
| Structured query language | Unstructured Query Language |
| databases have predefined schema | databases have dynamic schema for unstructured data
|

---

- What kind of data is a good fit for an SQL database?

> For the type of data to be stored: SQL databases are not best fit for hierarchical data storage.

---

- Give a real world example.

**MS-SQL Server Express Edition**

> It is a powerful and user friendly database which has good stability, reliability and scalability with support from Microsoft.

_The following are some of MS-SQL benefits and strengths:_

- Integrated Development Environment:

  - Microsoft visual studio, Sql Server Management Studio and Visual Developer tools provide a very helpful way for development and increase the developers productivity.

- Disaster Recovery:

  - It has good disaster recovery mechanism including database mirroring, fail over clustering and RAID partitioning.

- Cloud back-up:
  - Microsoft also provides cloud storage when you perform a cloud-backup of your database

---

- What kind of data is a good fit a NoSQL database?

> NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to **JSON data**. NoSQL database are **highly** preferred for **large data set**.

---

- Give a real world example.

**MongoDB**

> is one of the most popular document based NoSQL database as it stores data in JSON like documents. It is non-relational database with dynamic schema. It has been developed by the founders of DoubleClick, written in C++ and is currently being used by some big companies like The New York Times, Craigslist, MTV Networks.

_The following are some of MongoDB benefits and strengths:_

- Speed:

  - For simple queries, it gives good performance, as all the related data are in single document which eliminates the join operations.

- Scalability:

  - It is horizontally scalable i.e. you can reduce the workload by increasing the number of servers in your resource pool instead of relying on a stand alone resource.

- Manageable:

  - It is easy to use for both developers and administrators. This also gives the ability to shard database

- Dynamic Schema:
  - Its gives you the flexibility to evolve your data schema without modifying the existing data

---

- Which type of database is best for hierarchical data storage?

> NoSQL database fits better for the hierarchical data storage

---

Which type of database is best for scalability?

> NoSQL database fits better for the scalability

---

## sql vs nosql

- What does SQL stand for?

> `Structured Query Language`

---

- What is a realational database?

> A relational database is a type of database that stores and provides access to data points that are related to one another. The columns of the table hold attributes of the data, and each record usually has a value for each attribute, making it easy to establish the relationships among data points.

---

- What type of structure does a relational database work with?

> Relational Model.

The relational model means that the `logical data structures` the `data tables`, `views`,0 and `indexes` are separate from the physical storage structures.

     This separation means that database administrators can manage physical data storage without affecting access to that data as a logical structure.

---

- What is a ‘schema’?

> The term `"schema"` refers to the organization of data as a blueprint of how the database is constructed.

**that represents the storage of your data in a database.**

    It describes both the organization of data and the relationships between tables in a given database.

---

- What is a NoSQL database?

> A NoSQL originally referring to `"non-SQL"` or `"non-relational"` database provides a mechanism for storage and retrieval of data that is modeled in means other than the tabular relations used in relational databases.

---

- Howo does it work?

> The simplest type to describe is the document database, in which it would be natural to combine both the `basic information` and the `customer information` in **one** `JSON` document. In this case, each of the SQL column attributes would be fields and the details of a customer’s record would be the data values associated with each field.

---

- What is inside of a Mongo database?

> MongoDB stores data records as `documents` (specifically **BSON** documents) which are gathered together in collections.

        A database stores one or more collections of documents

---

- Which is more flexible - SQL or MongoDB? and why.

**MongoDB** is more flexible

> because Data in MongoDB has a flexible schema , it provides a flexible developer interface for teams that are building applications that don’t need all of the safety features offered by relational systems. This flexibility gives you data-modeling choices to match your application and its performance requirements.

---

- What is the disadvantage of a NoSQL database?

-> don’t have the reliability functions which Relational Databases have (basically don’t support ACID).

-> NoSQL is not compatible.

-> NoSQL are very new compared to Relational Databases, which means that are far less stable and may have a lot less functionalities.
