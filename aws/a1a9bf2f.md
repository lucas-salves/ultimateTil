# DynamoDB

Is a key/value serverless , encrypted, safe and elastic NoSQL database that supports transactions with high performance even in the more intense case uses.
DynamoDB has integrated resources of security, backup and restoration and memory cache storage.
The DynamoDB interactions are stateless, that means the applications doesn't need to keep persistant network connections, but only HTTP requests.
All the data is stored in SSDs and automatically replicated in different data-centers.

## Benefits
* High performance
* Serverless
* Elastic: grow and shrink tables automatically to adjust according to maintain the performance.
* High availability
* ACID: Supports atomicity, consistency, isolation and durability
* Security: encrypts all the data by default and allows refined control of access and identity to your tables
* Event friendly

## Components

* Tables
* Itens: each table have zero or more itens. A item is a group of attributes
* Attributes: each item it's composed by one or more attributes
* Nested Attributes: supports up to 32 nested attributes
* Schema
* Primary key
* Secondary indexes
* Global secondary index
* Local secondary index

## Capacity
DynamoDB has two ways of capacity of read/write to proccess read/write: on demand or provisioned

## Provisioned Capcacity
Its a good choice when you have previsible traffic.
Capacity Units (CUs) are the way AWS use to charge for its use. For each table in the database, you need to supply the Capacity Units of read (Read capacity unit) and write (write capacity unit).

One Read Capacity Unit represents a consistent read or two eventually consistent reads per second, to a item of 4KB.
A Write capacity unit represents one write per second to an item of 1 KB.

## On demand capacity

its elastic and suits automatically to growth and reduction of workloads

## Auto scaling
Manages the capacity of throughput of tables and secondary global indexes.

## Types of data
DynamoDB can hold different types of data to attributes within a table:
* Scalar types: represents a value like a number, string, binary, boolean or null
* Document types: complex structure of nested attributes, like a JSON file. The type of documents are List or Map.
* Set: represent several scalar types. The Set are a set of strings, set of numbers or set of binaries.

### References
- [DynamoDB: tudo o que você precisa saber para começar](https://blog.andrefaria.com/dynamodb-tudo-o-que-voce-precisa-saber-para-comecar)
