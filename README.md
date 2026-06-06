# Mongo-for-DevOps-Engineers

![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)

![](Mongo.png)

## Mongo Self Assessment

<details>
<summary><b><i>1.What are the advantages of MongoDB? Or in other words, why choosing MongoDB and not other implementation of NoSQL?</i></b></summary>

$\color{green}{\text{Answer}}$

MongoDB advantages are as following:

- Schemaless
- Easy to scale-out
- No complex joins
- Structure of a single object is clear

</details>

<details>
<summary><b><i>2.What is the difference between SQL and NoSQL?</i></b></summary>

$\color{green}{\text{Answer}}$

The main difference is that SQL databases are structured (data is stored in the form of tables with rows and columns - like an excel spreadsheet table) while NoSQL is unstructured, and the data storage can vary depending on how the NoSQL DB is set up, such as key-value pair, document-oriented, etc.

</details>

<details>
<summary><b><i>3.In what scenarios would you prefer to use NoSQL/Mongo over SQL?</i></b></summary>

$\color{green}{\text{Answer}}$

- Heterogeneous data which changes often
- Data consistency and integrity is not top priority
- Best if the database needs to scale rapidly

</details>

<details>
<summary><b><i>4.What is a document? What is a collection?</i></b></summary>

$\color{green}{\text{Answer}}$

- A document is a record in MongoDB, which is stored in BSON (Binary JSON) format and is the basic unit of data in MongoDB.
- A collection is a group of related documents stored in a single database in MongoDB.

</details>

<details>
<summary><b><i>5.What is an aggregator?</i></b></summary>

$\color{green}{\text{Answer}}$

An aggregator is a framework in MongoDB that performs operations on a set of data to return a single computed result.

</details>

<details>
<summary><b><i>6.What is better? Embedded documents or referenced?</i></b></summary>

$\color{green}{\text{Answer}}$

There is no definitive answer to which is better, it depends on the specific use case and requirements. Embedded documents provide atomic updates, while referenced documents allow for better normalization.

</details>

<details>
<summary><b><i>7.Have you performed data retrieval optimizations in Mongo? If not, can you think about ways to optimize a slow data retrieval?</i></b></summary>

$\color{green}{\text{Answer}}$

Some ways to optimize data retrieval in MongoDB are: indexing, proper schema design, query optimization and database load balancing.

</details>

## Queries

<details>
<summary><b><i>8.Explain this query: 
  
```Mongo
db.books.find({"name": /abc/})
```

</i></b></summary>

$\color{green}{\text{Answer}}$

This MongoDB query searches the `books` collection and returns all documents where the `name` field contains the exact sequence of letters `abc` anywhere within the string.

</details>

<details>
<summary><b><i>9.Explain this query: 
  
```Mongo
db.books.find().sort({x:1})
```

</i></b></summary>

$\color{green}{\text{Answer}}$

This MongoDB query retrieves all documents from the `books` collection and orders the results in ascending order based on the value of the `x` field.

</details>

<details>
<summary><b><i>10.What is the difference between find() and find_one()?</i></b></summary>

$\color{green}{\text{Answer}}$

- `find()` returns all documents that match the query conditions.
- `find_one()` returns only one document that matches the query conditions (or null if no match is found).

</details>

<details>
<summary><b><i>11.How can you export data from Mongo DB?</i></b></summary>

$\color{green}{\text{Answer}}$

- mongoexport
- programming languages

</details>
