# Mongo and Mongoose

## Nosql vs. SQL

 | SQL | NoSqul |
   | ----| ----- |
   |Table based databases| Key-value pair based databse |
   | Pre-deifined schema | Undefined schema for unstructured data |
   | Uses structured query languages to defining and manipulating datbases | Uses queries that are focused on a collection of documents |
   | Good fit for complex query intensive environments | Doon't have standard interfaces to perform complex queries |
   | More stable and promises mroe atomicity as well as integrity for the data | Not stable enough in high load for complex transactional applications |

1. **What kind of data is a good fit for for SQL databases?** Anything that can fit on a table or a spreadsheet is a good fit for a SQL database/

2. **Give a real world example.** Any kind of banking information I would assume would be a good fit, as it is common practice to track personal financial information on spreadsheets.

3. **What kind of data is a good fit a NoSQL database?** Anything stored in a JSON or JSON like file is a good fit for a NoSQL database.

4. **Give a real world example.** Any kind of large form or text like document sounds like it would be a good fit for the NoSQL format of database.

5. **Which type of database is best for hierarchical data storage?** NoSQL.

6. **Which type of database is best for scalability?** If you are stuck to one server: SQL. If you have access to multiple servers: NoSQL.

## Video

1. **What does SQL stand for?** Structured Query Language.

2. **What is a relational database?** A database that has certain assumptions about the data structure, and one that works with the SQ language.

3. **What type of structure does a relational database work with?** Tables.

4. **What is a ‘schema’?** A schema in the SQL definition is a table defined by fields or columns in which points of data are stored.

5. **What is a NoSQL database?** Instead of tables the information is stored in collections that are more or less large collections of JSON files. This lends itself to not having a schema and housing large amounts of data.

6. **How does it work?** Each collection holds enough information so that if you query that collection, you get enough information for that particular query. While there might be more detailed collections elsewhere with more information about the data stored within the collection you are querying, the one that you are querying has enough information so that you can complete the query.

7. **What is inside of a Mongo database?** A large collection of collections that house JSON like files.

8. **Which is more flexible - SQL or MongoDB? and why.** No SQL is more flexible because the data it houses doesn't exist in a schema, so it can be more easily edited.

9. **What is the disadvantage of a NoSQL database?** It is harder to edit that data stored within a NoSQL database because it doesn't exist in a table format.
