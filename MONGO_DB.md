# MongoDB Interview Questions & Answers — Complete Revision Guide

A complete, structured collection of MongoDB interview questions — from fundamental NoSQL concepts to indexing, aggregation, replication, sharding, and architecture — with clear answers and code examples where they help. Built to be your one-stop revision resource the night before an interview or test.

## 📚 Table of Contents

- [🔥 Most Asked / Tricky Questions](#most-asked-tricky-questions)
  - [What is MongoDB, and how does it differ from a relational database (RDBMS)?](#what-is-mongodb-and-how-does-it-differ-from-a-relational-database-rdbms)
  - [What is the difference between sharding and replication?](#what-is-the-difference-between-sharding-and-replication)
  - [What is the aggregation pipeline?](#what-is-the-aggregation-pipeline)
  - [What is the difference between embedding and referencing documents, and when would you use each?](#what-is-the-difference-between-embedding-and-referencing-documents-and-when-would-you-use-each)
  - [What types of indexes does MongoDB support?](#what-types-of-indexes-does-mongodb-support)
  - [How does MongoDB handle multi-document transactions?](#how-does-mongodb-handle-multi-document-transactions)
  - [What is BSON, and why does MongoDB use it instead of plain JSON?](#what-is-bson-and-why-does-mongodb-use-it-instead-of-plain-json)
  - [What is the `_id` field, and what is an `ObjectId`?](#what-is-the-id-field-and-what-is-an-objectid)
  - [How would you diagnose and optimize a slow MongoDB query?](#how-would-you-diagnose-and-optimize-a-slow-mongodb-query)
  - [What does the `explain()` method show, and why is it important?](#what-does-the-explain-method-show-and-why-is-it-important)
  - [What is the difference between write concern and read preference?](#what-is-the-difference-between-write-concern-and-read-preference)
  - [What are capped collections?](#what-are-capped-collections)
  - [How does MongoDB achieve high availability?](#how-does-mongodb-achieve-high-availability)
  - [What is a replica set?](#what-is-a-replica-set)
  - [What are TTL (Time To Live) indexes?](#what-are-ttl-time-to-live-indexes)
- [MongoDB Basics](#mongodb-basics)
  - [What is a NoSQL database, and how does MongoDB fit into that category?](#what-is-a-nosql-database-and-how-does-mongodb-fit-into-that-category)
  - [What are the core features of MongoDB?](#what-are-the-core-features-of-mongodb)
  - [What is the difference between a document and a collection?](#what-is-the-difference-between-a-document-and-a-collection)
  - [What is the Mongo Shell (`mongosh`)?](#what-is-the-mongo-shell-mongosh)
  - [What data types does MongoDB support in documents?](#what-data-types-does-mongodb-support-in-documents)
  - [What is the maximum size of a single MongoDB document?](#what-is-the-maximum-size-of-a-single-mongodb-document)
  - [What is `mongod`, and what is `mongos`?](#what-is-mongod-and-what-is-mongos)
  - [What is a namespace in MongoDB?](#what-is-a-namespace-in-mongodb)
  - [How does MongoDB handle schema flexibility, and what's a risk of that flexibility?](#how-does-mongodb-handle-schema-flexibility-and-whats-a-risk-of-that-flexibility)
  - [What is schema validation in MongoDB?](#what-is-schema-validation-in-mongodb)
  - [What is the difference between MongoDB Atlas and a self-hosted MongoDB deployment?](#what-is-the-difference-between-mongodb-atlas-and-a-self-hosted-mongodb-deployment)
  - [What are some common use cases where MongoDB is a strong fit?](#what-are-some-common-use-cases-where-mongodb-is-a-strong-fit)
- [CRUD Operations](#crud-operations)
  - [How do you insert documents into a MongoDB collection?](#how-do-you-insert-documents-into-a-mongodb-collection)
  - [What is the difference between `find()` and `findOne()`?](#what-is-the-difference-between-find-and-findone)
  - [How do you update documents in MongoDB, and what are common update operators?](#how-do-you-update-documents-in-mongodb-and-what-are-common-update-operators)
  - [What is the difference between `updateOne()` and `updateMany()`?](#what-is-the-difference-between-updateone-and-updatemany)
  - [How do you delete documents in MongoDB?](#how-do-you-delete-documents-in-mongodb)
  - [What is the difference between `updateOne()` and `replaceOne()`?](#what-is-the-difference-between-updateone-and-replaceone)
  - [What does the `upsert` option do in an update operation?](#what-does-the-upsert-option-do-in-an-update-operation)
  - [What is a projection, and how do you use one with `find()`?](#what-is-a-projection-and-how-do-you-use-one-with-find)
  - [How do you sort, limit, and skip results in a query?](#how-do-you-sort-limit-and-skip-results-in-a-query)
  - [What is the difference between `$set` and `$setOnInsert` update operators?](#what-is-the-difference-between-set-and-setoninsert-update-operators)
- [Indexing](#indexing)
  - [Why is indexing important in MongoDB?](#why-is-indexing-important-in-mongodb)
  - [What is a compound index, and does field order matter?](#what-is-a-compound-index-and-does-field-order-matter)
  - [What is a multikey index?](#what-is-a-multikey-index)
  - [What is a text index, and what is it used for?](#what-is-a-text-index-and-what-is-it-used-for)
  - [What is a geospatial index, and when would you use one?](#what-is-a-geospatial-index-and-when-would-you-use-one)
  - [What is a covered query?](#what-is-a-covered-query)
  - [What is the difference between a sparse index and a partial index?](#what-is-the-difference-between-a-sparse-index-and-a-partial-index)
  - [What is index intersection in MongoDB?](#what-is-index-intersection-in-mongodb)
  - [How do you view the indexes currently defined on a collection?](#how-do-you-view-the-indexes-currently-defined-on-a-collection)
  - [What is a unique index, and what happens if you try to violate it?](#what-is-a-unique-index-and-what-happens-if-you-try-to-violate-it)
- [Aggregation Framework](#aggregation-framework)
  - [What is the `$match` stage used for?](#what-is-the-match-stage-used-for)
  - [What does the `$group` stage do?](#what-does-the-group-stage-do)
  - [What is `$lookup`, and how is it used to perform joins?](#what-is-lookup-and-how-is-it-used-to-perform-joins)
  - [What do the `$project` and `$unwind` stages do?](#what-do-the-project-and-unwind-stages-do)
  - [Does MongoDB have a `$having` stage like SQL's `HAVING` clause?](#does-mongodb-have-a-having-stage-like-sqls-having-clause)
  - [What does the `$sort` stage do, and where should it typically be placed in a pipeline?](#what-does-the-sort-stage-do-and-where-should-it-typically-be-placed-in-a-pipeline)
  - [What is the `$facet` stage used for?](#what-is-the-facet-stage-used-for)
  - [What is the difference between `$addFields` and `$project`?](#what-is-the-difference-between-addfields-and-project)
  - [What accumulator operators are commonly used with `$group`?](#what-accumulator-operators-are-commonly-used-with-group)
  - [How would you compute a running/cumulative total using the aggregation pipeline?](#how-would-you-compute-a-runningcumulative-total-using-the-aggregation-pipeline)
- [Data Modeling & Schema Design](#data-modeling-schema-design)
  - [What does schema design mean in MongoDB, given it doesn't enforce a fixed schema?](#what-does-schema-design-mean-in-mongodb-given-it-doesnt-enforce-a-fixed-schema)
  - [What is the difference between normalization and denormalization, and how does MongoDB relate to each?](#what-is-the-difference-between-normalization-and-denormalization-and-how-does-mongodb-relate-to-each)
  - [What is GridFS, and when would you use it?](#what-is-gridfs-and-when-would-you-use-it)
  - [What is the "one-to-few," "one-to-many," and "one-to-squillions" pattern in schema design?](#what-is-the-one-to-few-one-to-many-and-one-to-squillions-pattern-in-schema-design)
  - [What is the "Subset Pattern" in MongoDB schema design?](#what-is-the-subset-pattern-in-mongodb-schema-design)
  - [What is the "Bucket Pattern," and what problem does it solve?](#what-is-the-bucket-pattern-and-what-problem-does-it-solve)
  - [How do you decide between embedding and referencing for a specific relationship?](#how-do-you-decide-between-embedding-and-referencing-for-a-specific-relationship)
  - [What is schema versioning, and why might you need it in MongoDB?](#what-is-schema-versioning-and-why-might-you-need-it-in-mongodb)
  - [What is the Extended Reference Pattern?](#what-is-the-extended-reference-pattern)
  - [How does MongoDB's document model affect how you'd model a many-to-many relationship, compared to a relational database?](#how-does-mongodbs-document-model-affect-how-youd-model-a-many-to-many-relationship-compared-to-a-relational-database)
- [Replication](#replication)
  - [How does replication work in MongoDB, step by step?](#how-does-replication-work-in-mongodb-step-by-step)
  - [What is the oplog, and why is it important?](#what-is-the-oplog-and-why-is-it-important)
  - [How does a replica set elect a new primary?](#how-does-a-replica-set-elect-a-new-primary)
  - [What is a replica set's write concern majority, and why is it recommended for critical writes?](#what-is-a-replica-sets-write-concern-majority-and-why-is-it-recommended-for-critical-writes)
  - [What is an arbiter in a replica set?](#what-is-an-arbiter-in-a-replica-set)
  - [What is replication lag, and why does it matter?](#what-is-replication-lag-and-why-does-it-matter)
  - [What is a hidden member in a replica set, and when would you use one?](#what-is-a-hidden-member-in-a-replica-set-and-when-would-you-use-one)
  - [Can you read from a secondary, and what are the trade-offs?](#can-you-read-from-a-secondary-and-what-are-the-trade-offs)
- [Sharding](#sharding)
  - [What is sharding, and what problem does it solve?](#what-is-sharding-and-what-problem-does-it-solve)
  - [What are the main components of a sharded cluster?](#what-are-the-main-components-of-a-sharded-cluster)
  - [What is a shard key, and why is choosing a good one important?](#what-is-a-shard-key-and-why-is-choosing-a-good-one-important)
  - [What is the difference between ranged sharding and hashed sharding?](#what-is-the-difference-between-ranged-sharding-and-hashed-sharding)
  - [What is a chunk in a sharded cluster?](#what-is-a-chunk-in-a-sharded-cluster)
  - [What is the balancer, and what does it do?](#what-is-the-balancer-and-what-does-it-do)
  - [Can you change a collection's shard key after sharding it?](#can-you-change-a-collections-shard-key-after-sharding-it)
  - [What is a jumbo chunk, and why is it a problem?](#what-is-a-jumbo-chunk-and-why-is-it-a-problem)
- [Transactions & Consistency](#transactions-consistency)
  - [Are single-document writes in MongoDB atomic even without an explicit transaction?](#are-single-document-writes-in-mongodb-atomic-even-without-an-explicit-transaction)
  - [What isolation guarantees do MongoDB transactions provide?](#what-isolation-guarantees-do-mongodb-transactions-provide)
  - [What are some downsides or limitations of using multi-document transactions in MongoDB?](#what-are-some-downsides-or-limitations-of-using-multi-document-transactions-in-mongodb)
  - [What is causal consistency in MongoDB?](#what-is-causal-consistency-in-mongodb)
  - [What does "read your own writes" mean in the context of MongoDB reads?](#what-does-read-your-own-writes-mean-in-the-context-of-mongodb-reads)
  - [What is a write concern of `w: 0`, and when (if ever) would you use it?](#what-is-a-write-concern-of-w-0-and-when-if-ever-would-you-use-it)
  - [What is a retryable write, and why is it useful?](#what-is-a-retryable-write-and-why-is-it-useful)
  - [What is the difference between optimistic and pessimistic concurrency control, and which does MongoDB favor?](#what-is-the-difference-between-optimistic-and-pessimistic-concurrency-control-and-which-does-mongodb-favor)
- [Security](#security)
  - [How do you enable authentication in MongoDB?](#how-do-you-enable-authentication-in-mongodb)
  - [What is Role-Based Access Control (RBAC) in MongoDB?](#what-is-role-based-access-control-rbac-in-mongodb)
  - [How do you secure data at rest in MongoDB?](#how-do-you-secure-data-at-rest-in-mongodb)
  - [What is the difference between authentication and authorization?](#what-is-the-difference-between-authentication-and-authorization)
  - [What mechanisms does MongoDB support for encrypting data in transit?](#what-mechanisms-does-mongodb-support-for-encrypting-data-in-transit)
  - [What is field-level encryption in MongoDB?](#what-is-field-level-encryption-in-mongodb)
  - [What is IP whitelisting, and why is it a recommended security practice for MongoDB?](#what-is-ip-whitelisting-and-why-is-it-a-recommended-security-practice-for-mongodb)
  - [What is the principle of least privilege, and how does it apply to MongoDB user roles?](#what-is-the-principle-of-least-privilege-and-how-does-it-apply-to-mongodb-user-roles)
- [Performance & Monitoring](#performance-monitoring)
  - [What is the Database Profiler, and how do you use it?](#what-is-the-database-profiler-and-how-do-you-use-it)
  - [What are common causes of MongoDB performance bottlenecks?](#what-are-common-causes-of-mongodb-performance-bottlenecks)
  - [What is the "working set," and why does it matter for performance?](#what-is-the-working-set-and-why-does-it-matter-for-performance)
  - [How would you monitor a MongoDB deployment in production?](#how-would-you-monitor-a-mongodb-deployment-in-production)
  - [What is `mongostat`, and what does it show?](#what-is-mongostat-and-what-does-it-show)
  - [What is index cardinality, and why does it matter for query performance?](#what-is-index-cardinality-and-why-does-it-matter-for-query-performance)
  - [What is connection pooling, and why is it important for MongoDB clients?](#what-is-connection-pooling-and-why-is-it-important-for-mongodb-clients)
  - [How would you identify and fix an inefficient query in a live production system?](#how-would-you-identify-and-fix-an-inefficient-query-in-a-live-production-system)
- [Common Coding Challenges](#common-coding-challenges)
  - [Write an aggregation query to find total sales per category.](#write-an-aggregation-query-to-find-total-sales-per-category)
  - [Implement simple pagination using `skip()` and `limit()`.](#implement-simple-pagination-using-skip-and-limit)
  - [Write a query to find the top 3 highest-paid employees in each department.](#write-a-query-to-find-the-top-3-highest-paid-employees-in-each-department)
  - [Write a query to find documents where an array field contains a specific value.](#write-a-query-to-find-documents-where-an-array-field-contains-a-specific-value)
  - [Write an update that increments a counter field and pushes a value onto an array in a single operation.](#write-an-update-that-increments-a-counter-field-and-pushes-a-value-onto-an-array-in-a-single-operation)
  - [Write a query using `$lookup` to join orders with their corresponding customer details.](#write-a-query-using-lookup-to-join-orders-with-their-corresponding-customer-details)
  - [Write a query to find and remove duplicate documents based on a field, keeping only one copy.](#write-a-query-to-find-and-remove-duplicate-documents-based-on-a-field-keeping-only-one-copy)
  - [Write a query that performs a case-insensitive search on a text field.](#write-a-query-that-performs-a-case-insensitive-search-on-a-text-field)
  - [Write an aggregation to calculate the average order value per month.](#write-an-aggregation-to-calculate-the-average-order-value-per-month)
  - [Write a query to atomically find a document, update it, and return the updated version.](#write-a-query-to-atomically-find-a-document-update-it-and-return-the-updated-version)
- [Behavioral / Scenario-Based Questions](#behavioral-scenario-based-questions)
  - [How would you migrate an existing relational (SQL) database to MongoDB?](#how-would-you-migrate-an-existing-relational-sql-database-to-mongodb)
  - [How would you design a schema for a high-write-volume application, like an IoT sensor logging system?](#how-would-you-design-a-schema-for-a-high-write-volume-application-like-an-iot-sensor-logging-system)
  - [A collection's queries are slow despite having what looks like a reasonable index — how would you investigate?](#a-collections-queries-are-slow-despite-having-what-looks-like-a-reasonable-index-how-would-you-investigate)
  - [How would you handle a scenario where a shard key choice turns out to be causing uneven load across shards?](#how-would-you-handle-a-scenario-where-a-shard-key-choice-turns-out-to-be-causing-uneven-load-across-shards)
  - [How would you approach designing a MongoDB schema for a social media application's posts and comments?](#how-would-you-approach-designing-a-mongodb-schema-for-a-social-media-applications-posts-and-comments)
  - [How would you ensure data consistency when updating related data across two collections, given MongoDB doesn't enforce foreign key constraints?](#how-would-you-ensure-data-consistency-when-updating-related-data-across-two-collections-given-mongodb-doesnt-enforce-foreign-key-constraints)
  - [How would you approach capacity planning before sharding a growing MongoDB deployment?](#how-would-you-approach-capacity-planning-before-sharding-a-growing-mongodb-deployment)
  - [How would you approach reviewing a teammate's proposed MongoDB schema in a design review?](#how-would-you-approach-reviewing-a-teammates-proposed-mongodb-schema-in-a-design-review)
- [How to Use This Guide](#how-to-use-this-guide)

---

<a id="most-asked-tricky-questions"></a>
## 🔥 Most Asked / Tricky Questions

These come up in almost every MongoDB interview. If you're short on time, start here.

<a id="what-is-mongodb-and-how-does-it-differ-from-a-relational-database-rdbms"></a>
### Q: What is MongoDB, and how does it differ from a relational database (RDBMS)?
**Answer:** MongoDB is a NoSQL, document-oriented database that stores data as flexible, JSON-like BSON documents grouped into collections, rather than rows in fixed-schema tables. Unlike an RDBMS, documents in the same collection can have different fields (a dynamic schema), it scales horizontally via sharding rather than primarily vertically, and relationships are typically modeled through embedding or application-level references instead of SQL joins.

<a id="what-is-the-difference-between-sharding-and-replication"></a>
### Q: What is the difference between sharding and replication?
**Answer:** Replication copies the same data across multiple servers (a replica set) purely for redundancy and high availability — if the primary node fails, a secondary is elected to take over. Sharding instead splits different pieces of data across multiple servers (shards) to scale horizontally, so no single server needs to hold the entire dataset. They solve different problems and are commonly used together in production.

<a id="what-is-the-aggregation-pipeline"></a>
### Q: What is the aggregation pipeline?
**Answer:** The aggregation pipeline processes documents through a sequence of stages (`$match`, `$group`, `$sort`, `$project`, etc.), where each stage transforms the documents and passes its output to the next — similar in spirit to a Unix pipe, letting you build complex data transformations, filtering, and analytics in one query.

<a id="what-is-the-difference-between-embedding-and-referencing-documents-and-when-would-you-use-each"></a>
### Q: What is the difference between embedding and referencing documents, and when would you use each?
**Answer:** Embedding nests related data directly inside a single document — best for one-to-few relationships and data almost always read together, since it avoids extra queries and keeps related data co-located. Referencing stores related data in a separate collection linked via an `_id` reference — better for one-to-many or many-to-many relationships, data that grows unbounded, or data reused across many parent documents, avoiding duplication and the 16MB document size limit.

<a id="what-types-of-indexes-does-mongodb-support"></a>
### Q: What types of indexes does MongoDB support?
**Answer:** Single-field, compound (multiple fields), multikey (indexing array field values), text (full-text search), geospatial (`2dsphere`/`2d` for location queries), hashed (for even shard-key distribution), wildcard, and TTL (automatically expiring documents after a set time).

<a id="how-does-mongodb-handle-multi-document-transactions"></a>
### Q: How does MongoDB handle multi-document transactions?
**Answer:** Since version 4.0, MongoDB supports multi-document ACID transactions on replica sets (extended to sharded clusters in 4.2), using a session object to start, commit, or abort a transaction across multiple operations/collections — though transactions carry more performance overhead than single-document writes, which are already atomic by default.

**Example:**
```js
const session = client.startSession();
session.startTransaction();
try {
  await collA.insertOne({ name: 'A' }, { session });
  await collB.insertOne({ name: 'B' }, { session });
  await session.commitTransaction();
} catch (err) {
  await session.abortTransaction();
} finally {
  session.endSession();
}
```

<a id="what-is-bson-and-why-does-mongodb-use-it-instead-of-plain-json"></a>
### Q: What is BSON, and why does MongoDB use it instead of plain JSON?
**Answer:** BSON (Binary JSON) is a binary-encoded serialization format MongoDB uses internally to store documents. It's more efficient to parse and traverse than text-based JSON, and it supports additional data types JSON lacks natively — like `Date`, `ObjectId`, and binary data.

<a id="what-is-the-id-field-and-what-is-an-objectid"></a>
### Q: What is the `_id` field, and what is an `ObjectId`?
**Answer:** Every document must have a unique `_id` field acting as its primary key — if you don't supply one, MongoDB auto-generates an `ObjectId`. An `ObjectId` is a 12-byte value made up of a 4-byte timestamp, a 5-byte random value unique per machine/process, and a 3-byte incrementing counter, making it roughly sortable by creation time and unique without coordination.

<a id="how-would-you-diagnose-and-optimize-a-slow-mongodb-query"></a>
### Q: How would you diagnose and optimize a slow MongoDB query?
**Answer:** Run `.explain("executionStats")` on the query to see whether it used an index or fell back to a full collection scan (`COLLSCAN`), add or adjust indexes to match the query's filter/sort fields, use projection to return only needed fields, avoid patterns that defeat index usage (like a leading-wildcard regex or negation operators), and check whether the working set fits comfortably in available RAM.

<a id="what-does-the-explain-method-show-and-why-is-it-important"></a>
### Q: What does the `explain()` method show, and why is it important?
**Answer:** `explain()` returns details of how MongoDB actually executed a query — whether it used an index (`IXSCAN`) or scanned the whole collection (`COLLSCAN`), how many documents were examined vs. returned, and execution time — essential for diagnosing and fixing slow queries.

**Example:**
```js
db.users.find({ age: { $gt: 25 } }).explain('executionStats');
```

<a id="what-is-the-difference-between-write-concern-and-read-preference"></a>
### Q: What is the difference between write concern and read preference?
**Answer:** Write concern controls how many replica set members must acknowledge a write before it's considered successful (e.g. `w: 1` for just the primary, `w: 'majority'` for most nodes) — a durability/safety trade-off. Read preference controls which replica set member(s) a read operation is routed to (`primary`, `secondary`, `nearest`, etc.) — a trade-off between read consistency and distributing load or reducing latency.

<a id="what-are-capped-collections"></a>
### Q: What are capped collections?
**Answer:** Fixed-size collections that maintain documents in insertion order and automatically overwrite the oldest documents once the collection reaches its maximum size — well suited to use cases like logging or caching recent events where old data can be discarded.

<a id="how-does-mongodb-achieve-high-availability"></a>
### Q: How does MongoDB achieve high availability?
**Answer:** Through replica sets — a group of `mongod` instances holding the same data, with one primary accepting all writes and secondaries continuously replicating from it. If the primary becomes unavailable, the remaining eligible members automatically hold an election to promote a new primary, minimizing downtime.

<a id="what-is-a-replica-set"></a>
### Q: What is a replica set?
**Answer:** A cluster of MongoDB nodes maintaining identical copies of the same data set — one primary node handles all writes, while secondary nodes asynchronously replicate the primary's oplog and can serve reads depending on read preference, providing redundancy and automatic failover.

<a id="what-are-ttl-time-to-live-indexes"></a>
### Q: What are TTL (Time To Live) indexes?
**Answer:** A special single-field index that automatically deletes documents from a collection once a specified number of seconds has passed since a stored timestamp field — commonly used for expiring session data, temporary tokens, or cached entries without needing a separate cleanup job.

**Example:**
```js
db.sessions.createIndex({ createdAt: 1 }, { expireAfterSeconds: 3600 });
```

---

<a id="mongodb-basics"></a>
## MongoDB Basics

<a id="what-is-a-nosql-database-and-how-does-mongodb-fit-into-that-category"></a>
### Q: What is a NoSQL database, and how does MongoDB fit into that category?
**Answer:** NoSQL ("not only SQL") databases store and retrieve data using models other than the fixed, tabular structure of relational databases — including document, key-value, column-family, and graph models. MongoDB is specifically a document-oriented NoSQL database, storing data as flexible BSON documents rather than rows in rigid tables.

<a id="what-are-the-core-features-of-mongodb"></a>
### Q: What are the core features of MongoDB?
**Answer:** A dynamic, flexible document schema; a rich query language and aggregation framework; built-in high availability via replica sets; horizontal scalability via sharding; and support for a wide range of index types for query performance.

<a id="what-is-the-difference-between-a-document-and-a-collection"></a>
### Q: What is the difference between a document and a collection?
**Answer:** A document is a single BSON record — MongoDB's basic unit of data, roughly analogous to a row in a relational table. A collection is a group of documents, roughly analogous to a table, though documents within one collection aren't required to share the same fields/schema.

<a id="what-is-the-mongo-shell-mongosh"></a>
### Q: What is the Mongo Shell (`mongosh`)?
**Answer:** An interactive JavaScript-based command-line interface for connecting to and interacting with a MongoDB server — running queries, inserting/updating/deleting data, and performing administrative tasks like creating indexes or users directly.

<a id="what-data-types-does-mongodb-support-in-documents"></a>
### Q: What data types does MongoDB support in documents?
**Answer:** Common BSON types include String, Integer, Double, Boolean, Date, ObjectId, Array, embedded Object (sub-document), Null, Binary data, Timestamp, and Decimal128, among others — a richer set than plain JSON's basic types.

<a id="what-is-the-maximum-size-of-a-single-mongodb-document"></a>
### Q: What is the maximum size of a single MongoDB document?
**Answer:** 16MB per document — a limit designed to keep documents efficient to transmit and keep entirely in memory. If a use case needs to store larger binary data (like files), MongoDB provides GridFS to split it into smaller chunks across multiple documents.

<a id="what-is-mongod-and-what-is-mongos"></a>
### Q: What is `mongod`, and what is `mongos`?
**Answer:** `mongod` is the core MongoDB database server process that actually stores data and handles queries. `mongos` is a lightweight query router used specifically in sharded cluster deployments — it sits in front of the shards, routing client requests to the correct shard(s) without storing data itself.

<a id="what-is-a-namespace-in-mongodb"></a>
### Q: What is a namespace in MongoDB?
**Answer:** The combination of a database name and a collection name, written as `database.collection` — it uniquely identifies a specific collection within a specific database on a server.

<a id="how-does-mongodb-handle-schema-flexibility-and-whats-a-risk-of-that-flexibility"></a>
### Q: How does MongoDB handle schema flexibility, and what's a risk of that flexibility?
**Answer:** Since collections don't enforce a fixed schema by default, documents can vary in structure — useful for evolving data models without migrations. The risk is inconsistent or messy data creeping in over time without discipline, which is why MongoDB also offers optional schema validation rules you can apply to a collection.

<a id="what-is-schema-validation-in-mongodb"></a>
### Q: What is schema validation in MongoDB?
**Answer:** An optional feature letting you define rules (via JSON Schema syntax) that documents must satisfy to be inserted or updated in a collection — giving you some of the structure/safety benefits of a fixed schema while still keeping the underlying flexibility MongoDB is known for.

<a id="what-is-the-difference-between-mongodb-atlas-and-a-self-hosted-mongodb-deployment"></a>
### Q: What is the difference between MongoDB Atlas and a self-hosted MongoDB deployment?
**Answer:** MongoDB Atlas is MongoDB's official fully-managed cloud database service — handling provisioning, scaling, backups, and patching for you across major cloud providers. A self-hosted deployment means running and managing `mongod`/`mongos` processes yourself on your own infrastructure, with full control but full operational responsibility too.

<a id="what-are-some-common-use-cases-where-mongodb-is-a-strong-fit"></a>
### Q: What are some common use cases where MongoDB is a strong fit?
**Answer:** Content management systems, product catalogs with varying attributes per item, real-time analytics, IoT/event data ingestion, and applications with rapidly evolving data models — generally, workloads that benefit from flexible schemas and horizontal scalability over strict relational integrity and complex multi-table joins.

---

<a id="crud-operations"></a>
## CRUD Operations

<a id="how-do-you-insert-documents-into-a-mongodb-collection"></a>
### Q: How do you insert documents into a MongoDB collection?
**Answer:** Use `insertOne()` for a single document, or `insertMany()` for multiple documents at once in a single call.

**Example:**
```js
db.users.insertOne({ name: 'John', age: 30 });
db.users.insertMany([{ name: 'A' }, { name: 'B' }]);
```

<a id="what-is-the-difference-between-find-and-findone"></a>
### Q: What is the difference between `find()` and `findOne()`?
**Answer:** `find()` returns a cursor over ALL documents matching the query, which you can then iterate, sort, or limit. `findOne()` returns just the single first matching document directly (or `null` if none match), without needing to handle a cursor.

<a id="how-do-you-update-documents-in-mongodb-and-what-are-common-update-operators"></a>
### Q: How do you update documents in MongoDB, and what are common update operators?
**Answer:** Use `updateOne()`, `updateMany()`, or `replaceOne()`, typically combined with update operators like `$set` (set a field's value), `$inc` (increment a number), `$push` (add to an array), or `$unset` (remove a field).

**Example:**
```js
db.users.updateOne({ name: 'John' }, { $set: { age: 31 } });
```

<a id="what-is-the-difference-between-updateone-and-updatemany"></a>
### Q: What is the difference between `updateOne()` and `updateMany()`?
**Answer:** `updateOne()` modifies only the first document that matches the filter. `updateMany()` modifies every document matching the filter.

<a id="how-do-you-delete-documents-in-mongodb"></a>
### Q: How do you delete documents in MongoDB?
**Answer:** Use `deleteOne()` to remove the first matching document, or `deleteMany()` to remove all matching documents.

**Example:**
```js
db.users.deleteMany({ status: 'inactive' });
```

<a id="what-is-the-difference-between-updateone-and-replaceone"></a>
### Q: What is the difference between `updateOne()` and `replaceOne()`?
**Answer:** `updateOne()` (with operators like `$set`) modifies only the specified fields, leaving the rest of the document untouched. `replaceOne()` replaces the ENTIRE matched document with a new one you provide — any fields not included in the replacement are lost.

<a id="what-does-the-upsert-option-do-in-an-update-operation"></a>
### Q: What does the `upsert` option do in an update operation?
**Answer:** Setting `{ upsert: true }` makes the operation insert a new document (based on the filter and update) if no document matches the filter, instead of doing nothing — combining "update if exists, otherwise insert" into a single call.

**Example:**
```js
db.users.updateOne({ email: 'a@b.com' }, { $set: { name: 'A' } }, { upsert: true });
```

<a id="what-is-a-projection-and-how-do-you-use-one-with-find"></a>
### Q: What is a projection, and how do you use one with `find()`?
**Answer:** A projection specifies which fields to include or exclude in the returned documents, reducing the amount of data transferred and processed. Pass it as the second argument to `find()`.

**Example:**
```js
db.users.find({ age: { $gt: 18 } }, { name: 1, email: 1, _id: 0 });
```

<a id="how-do-you-sort-limit-and-skip-results-in-a-query"></a>
### Q: How do you sort, limit, and skip results in a query?
**Answer:** Chain `.sort({ field: 1 or -1 })`, `.limit(n)`, and `.skip(n)` onto a `find()` cursor — `1` sorts ascending, `-1` descending.

**Example:**
```js
db.products.find().sort({ price: -1 }).skip(10).limit(10);
```

<a id="what-is-the-difference-between-set-and-setoninsert-update-operators"></a>
### Q: What is the difference between `$set` and `$setOnInsert` update operators?
**Answer:** `$set` always sets the specified field's value, whether the document is being updated or newly inserted via upsert. `$setOnInsert` only applies its values when the operation actually results in a NEW document being inserted via upsert — it's ignored if an existing document is matched and updated instead.

---

<a id="indexing"></a>
## Indexing

<a id="why-is-indexing-important-in-mongodb"></a>
### Q: Why is indexing important in MongoDB?
**Answer:** Without an index, MongoDB must perform a full collection scan — examining every document — to satisfy a query. An index lets MongoDB efficiently locate matching documents using a much smaller, ordered data structure, dramatically speeding up queries, sorts, and lookups on large collections.

<a id="what-is-a-compound-index-and-does-field-order-matter"></a>
### Q: What is a compound index, and does field order matter?
**Answer:** An index on multiple fields together. Field order matters a great deal — a compound index can efficiently support queries filtering on a prefix of its fields (in the same order), but not queries that skip the first field(s) or use a different order.

**Example:**
```js
db.products.createIndex({ category: 1, price: -1 });
```

<a id="what-is-a-multikey-index"></a>
### Q: What is a multikey index?
**Answer:** An index created automatically when you index a field that holds an array — MongoDB creates a separate index entry for each element of the array, letting queries efficiently match against any value contained within it.

<a id="what-is-a-text-index-and-what-is-it-used-for"></a>
### Q: What is a text index, and what is it used for?
**Answer:** A special index type supporting full-text search across string content in one or more fields, enabling operators like `$text` with `$search` to find documents containing specific words, with basic relevance-based ranking.

<a id="what-is-a-geospatial-index-and-when-would-you-use-one"></a>
### Q: What is a geospatial index, and when would you use one?
**Answer:** An index (`2dsphere` for spherical/Earth-like coordinates, or `2d` for flat planes) supporting location-based queries — like finding documents within a certain radius of a point, or sorted by nearest distance — used for location-aware features like store locators or ride-hailing apps.

<a id="what-is-a-covered-query"></a>
### Q: What is a covered query?
**Answer:** A query where all the fields it requests and filters on are entirely contained within an index, meaning MongoDB can satisfy the whole query directly from the index alone, without ever needing to read the actual documents from the collection — significantly faster.

<a id="what-is-the-difference-between-a-sparse-index-and-a-partial-index"></a>
### Q: What is the difference between a sparse index and a partial index?
**Answer:** A sparse index only includes documents that actually have the indexed field present, skipping documents missing that field entirely. A partial index — the more modern, flexible option — includes documents based on any specified filter expression, not just field existence, giving finer control over which documents get indexed.

<a id="what-is-index-intersection-in-mongodb"></a>
### Q: What is index intersection in MongoDB?
**Answer:** MongoDB's ability to use two or more existing single-field indexes together to satisfy a single query, instead of requiring one perfect compound index for every possible query combination — though a well-designed compound index is usually still more efficient than relying on intersection.

<a id="how-do-you-view-the-indexes-currently-defined-on-a-collection"></a>
### Q: How do you view the indexes currently defined on a collection?
**Answer:** Use `db.collectionName.getIndexes()` to list all indexes on that collection, including their fields, order, and any options like uniqueness or TTL expiration.

<a id="what-is-a-unique-index-and-what-happens-if-you-try-to-violate-it"></a>
### Q: What is a unique index, and what happens if you try to violate it?
**Answer:** A unique index ensures no two documents in the collection can have the same value for the indexed field(s), or combination for a compound unique index — inserting or updating a document that would create a duplicate throws a duplicate key error and the operation fails.

**Example:**
```js
db.users.createIndex({ email: 1 }, { unique: true });
```

---

<a id="aggregation-framework"></a>
## Aggregation Framework

<a id="what-is-the-match-stage-used-for"></a>
### Q: What is the `$match` stage used for?
**Answer:** It filters documents, passing along only those matching the specified condition(s) to the next stage in the pipeline — functionally similar to a `find()` query's filter, and best placed early in a pipeline to reduce the number of documents processed by later stages.

<a id="what-does-the-group-stage-do"></a>
### Q: What does the `$group` stage do?
**Answer:** It groups incoming documents by a specified key expression (via `_id`) and computes aggregate values (like `$sum`, `$avg`, `$max`, `$push`) across each group — similar to SQL's `GROUP BY` combined with aggregate functions.

**Example:**
```js
db.orders.aggregate([
  { $group: { _id: '$customerId', total: { $sum: '$amount' } } }
]);
```

<a id="what-is-lookup-and-how-is-it-used-to-perform-joins"></a>
### Q: What is `$lookup`, and how is it used to perform joins?
**Answer:** `$lookup` performs a left outer join against another collection in the same database, matching a local field to a foreign field and adding the matched documents as an array field on each output document — MongoDB's closest equivalent to a SQL join.

**Example:**
```js
db.orders.aggregate([
  { $lookup: { from: 'inventory', localField: 'item', foreignField: 'sku', as: 'inventoryDocs' } }
]);
```

<a id="what-do-the-project-and-unwind-stages-do"></a>
### Q: What do the `$project` and `$unwind` stages do?
**Answer:** `$project` reshapes each document — including, excluding, renaming, or computing new fields — similar to a projection in `find()` but with more transformation power. `$unwind` deconstructs an array field, outputting one separate document per array element, useful before further per-element processing or grouping.

<a id="does-mongodb-have-a-having-stage-like-sqls-having-clause"></a>
### Q: Does MongoDB have a `$having` stage like SQL's `HAVING` clause?
**Answer:** No — instead, you simply use a SECOND `$match` stage placed AFTER a `$group` stage to filter on aggregated/computed values, which serves the same purpose SQL's `HAVING` clause does after a `GROUP BY`.

<a id="what-does-the-sort-stage-do-and-where-should-it-typically-be-placed-in-a-pipeline"></a>
### Q: What does the `$sort` stage do, and where should it typically be placed in a pipeline?
**Answer:** It sorts documents by specified field(s), ascending (`1`) or descending (`-1`). Placing `$sort` after an early `$match` reduces the number of documents that need sorting, and placing it before a `$limit` lets MongoDB potentially optimize the two together (a top-N sort).

<a id="what-is-the-facet-stage-used-for"></a>
### Q: What is the `$facet` stage used for?
**Answer:** It runs multiple independent aggregation sub-pipelines within a single overall pipeline, each producing its own separate output field — useful for computing several different summaries (like paginated results AND a total count) from the same input documents in a single round trip.

<a id="what-is-the-difference-between-addfields-and-project"></a>
### Q: What is the difference between `$addFields` and `$project`?
**Answer:** `$addFields` adds new computed fields to each document while keeping all existing fields intact. `$project` requires you to explicitly specify every field you want to keep or exclude — anything not mentioned is dropped by default, giving more explicit control over the final output shape.

<a id="what-accumulator-operators-are-commonly-used-with-group"></a>
### Q: What accumulator operators are commonly used with `$group`?
**Answer:** `$sum` (total), `$avg` (average), `$min`/`$max`, `$push` (collect values into an array, keeping duplicates), `$addToSet` (collect unique values into an array), and `$first`/`$last` (relative to document order within the group).

<a id="how-would-you-compute-a-runningcumulative-total-using-the-aggregation-pipeline"></a>
### Q: How would you compute a running/cumulative total using the aggregation pipeline?
**Answer:** Use the `$setWindowFields` stage (available since MongoDB 5.0), specifying a `partitionBy`, a sort order, and a window function like `$sum` over a range of preceding documents — letting you compute cumulative sums, moving averages, and similar windowed calculations directly within the pipeline.

---

<a id="data-modeling-schema-design"></a>
## Data Modeling & Schema Design

<a id="what-does-schema-design-mean-in-mongodb-given-it-doesnt-enforce-a-fixed-schema"></a>
### Q: What does schema design mean in MongoDB, given it doesn't enforce a fixed schema?
**Answer:** Even without a database-enforced schema, an application still has an implicit data shape it relies on. Schema design in MongoDB is about deliberately choosing how to structure documents — what to embed vs. reference, how to group related data — based on your application's actual query and update patterns, rather than a rigid, normalized relational structure.

<a id="what-is-the-difference-between-normalization-and-denormalization-and-how-does-mongodb-relate-to-each"></a>
### Q: What is the difference between normalization and denormalization, and how does MongoDB relate to each?
**Answer:** Normalization splits data into separate, non-redundant tables/collections linked by references, minimizing duplication — the traditional relational approach. Denormalization duplicates or embeds related data together to optimize for read performance, at the cost of some data redundancy. MongoDB's document model naturally leans toward denormalization (embedding) where it fits the access pattern.

<a id="what-is-gridfs-and-when-would-you-use-it"></a>
### Q: What is GridFS, and when would you use it?
**Answer:** GridFS is a specification for storing and retrieving files larger than the 16MB document size limit, by splitting a file into smaller chunks stored across multiple documents in two collections (`fs.files` for metadata, `fs.chunks` for the binary data) — useful for storing images, videos, or other large binary assets directly in MongoDB.

<a id="what-is-the-one-to-few-one-to-many-and-one-to-squillions-pattern-in-schema-design"></a>
### Q: What is the "one-to-few," "one-to-many," and "one-to-squillions" pattern in schema design?
**Answer:** These describe relationship cardinality and guide the embed-vs-reference decision. One-to-few (a handful of related items) usually favors embedding directly. One-to-many (a moderate, bounded number) can go either way depending on access patterns. One-to-squillions (an effectively unbounded number, like a sensor logging millions of readings) should always use references, since embedding would blow past the document size limit.

<a id="what-is-the-subset-pattern-in-mongodb-schema-design"></a>
### Q: What is the "Subset Pattern" in MongoDB schema design?
**Answer:** A pattern where you embed only a small, frequently-accessed subset of a related large array (e.g. the 10 most recent reviews) directly in the parent document for fast, common-case reads, while storing the full set of related data in a separate collection for less-frequent, complete access.

<a id="what-is-the-bucket-pattern-and-what-problem-does-it-solve"></a>
### Q: What is the "Bucket Pattern," and what problem does it solve?
**Answer:** A pattern that groups many small, similar documents (like time-series sensor readings within an hour) into a single larger "bucket" document containing an array of readings, instead of storing one document per reading — reducing index overhead and document count for high-volume, append-heavy data.

<a id="how-do-you-decide-between-embedding-and-referencing-for-a-specific-relationship"></a>
### Q: How do you decide between embedding and referencing for a specific relationship?
**Answer:** Consider how often the related data is read together (embedding favors "read together, write together"), how large or unbounded the related data can grow (large/unbounded favors referencing), how often it changes independently (frequently-changing shared data favors referencing to avoid update-everywhere problems), and whether the 16MB document limit could realistically be hit.

<a id="what-is-schema-versioning-and-why-might-you-need-it-in-mongodb"></a>
### Q: What is schema versioning, and why might you need it in MongoDB?
**Answer:** As an application evolves, its document shape often needs to change over time. Schema versioning means including a version field (or inferring version from field presence) in documents, so application code can handle documents written under an older shape gracefully — since MongoDB doesn't force a migration of existing documents when your code's expected shape changes.

<a id="what-is-the-extended-reference-pattern"></a>
### Q: What is the Extended Reference Pattern?
**Answer:** A pattern where you embed just the frequently-needed fields of a referenced document (not the whole document) directly alongside the reference itself — e.g. storing a customer's name and email alongside an order, in addition to a reference to the full customer document — avoiding an extra lookup for the common case while still keeping the full related data in its own collection.

<a id="how-does-mongodbs-document-model-affect-how-youd-model-a-many-to-many-relationship-compared-to-a-relational-database"></a>
### Q: How does MongoDB's document model affect how you'd model a many-to-many relationship, compared to a relational database?
**Answer:** A relational database typically models many-to-many via a separate join table. In MongoDB, you'd commonly instead store an array of references (IDs) on one or both sides of the relationship directly within the documents themselves, resolving the "join" at query time via `$lookup` or multiple queries in application code, rather than maintaining a dedicated junction collection.

---

<a id="replication"></a>
## Replication

<a id="how-does-replication-work-in-mongodb-step-by-step"></a>
### Q: How does replication work in MongoDB, step by step?
**Answer:** The primary node records every write operation in a special capped collection called the oplog (operations log). Secondary nodes continuously read and apply operations from the primary's oplog to keep their own data in sync, applying them in the same order they occurred on the primary.

<a id="what-is-the-oplog-and-why-is-it-important"></a>
### Q: What is the oplog, and why is it important?
**Answer:** The oplog (operations log) is a capped collection on the primary that records every write operation applied to the database, in order. Secondaries replicate by tailing and reapplying this log — it's also central to point-in-time recovery and certain backup strategies.

<a id="how-does-a-replica-set-elect-a-new-primary"></a>
### Q: How does a replica set elect a new primary?
**Answer:** If the current primary becomes unreachable, the remaining eligible secondaries hold an election, each casting votes based on factors like how up-to-date their replicated data is and any configured member priorities — the member that wins majority support is promoted to primary, typically within seconds.

<a id="what-is-a-replica-sets-write-concern-majority-and-why-is-it-recommended-for-critical-writes"></a>
### Q: What is a replica set's write concern majority, and why is it recommended for critical writes?
**Answer:** `{ w: 'majority' }` requires a write to be acknowledged by a majority of voting replica set members before it's considered successful, ensuring the write has been durably replicated and is very unlikely to be rolled back even if the current primary subsequently fails.

<a id="what-is-an-arbiter-in-a-replica-set"></a>
### Q: What is an arbiter in a replica set?
**Answer:** A replica set member that participates in elections (casting a vote) but doesn't hold a copy of the data itself — used to maintain an odd number of voting members, needed for clean majority elections, without the cost of a full additional data-bearing node.

<a id="what-is-replication-lag-and-why-does-it-matter"></a>
### Q: What is replication lag, and why does it matter?
**Answer:** The delay between when a write happens on the primary and when a secondary has actually applied that same write. High replication lag matters because reads directed to a lagging secondary (depending on read preference) could return stale data, and a large lag also increases the risk of data loss if the primary fails before a slow secondary catches up.

<a id="what-is-a-hidden-member-in-a-replica-set-and-when-would-you-use-one"></a>
### Q: What is a hidden member in a replica set, and when would you use one?
**Answer:** A replica set member that replicates data like any secondary but is invisible to client applications — never receives reads or becomes primary — commonly used for dedicated backup or reporting/analytics workloads that shouldn't compete with production traffic.

<a id="can-you-read-from-a-secondary-and-what-are-the-trade-offs"></a>
### Q: Can you read from a secondary, and what are the trade-offs?
**Answer:** Yes, by setting an appropriate read preference (e.g. `secondary` or `secondaryPreferred`). The trade-off is potentially reading slightly stale data due to replication lag, in exchange for distributing read load away from the primary and potentially lower latency if a secondary is geographically closer to the client.

---

<a id="sharding"></a>
## Sharding

<a id="what-is-sharding-and-what-problem-does-it-solve"></a>
### Q: What is sharding, and what problem does it solve?
**Answer:** Sharding partitions a collection's data across multiple servers (shards) based on a shard key, letting a dataset and its read/write throughput scale horizontally beyond what a single server could handle — necessary when data volume or load outgrows a single machine's capacity.

<a id="what-are-the-main-components-of-a-sharded-cluster"></a>
### Q: What are the main components of a sharded cluster?
**Answer:** Shards (each holding a subset of the data, typically as its own replica set for redundancy), `mongos` query routers (route client requests to the correct shard(s), with no data of their own), and config servers (store the cluster's metadata — which data ranges live on which shard).

<a id="what-is-a-shard-key-and-why-is-choosing-a-good-one-important"></a>
### Q: What is a shard key, and why is choosing a good one important?
**Answer:** The field (or fields) used to determine how a collection's documents are distributed across shards. A poorly chosen shard key can lead to uneven data distribution ("hotspotting" one shard) or uneven write load concentrated on a single shard, while a well-chosen key spreads both data and traffic evenly across the cluster.

<a id="what-is-the-difference-between-ranged-sharding-and-hashed-sharding"></a>
### Q: What is the difference between ranged sharding and hashed sharding?
**Answer:** Ranged sharding groups documents with similar shard key values together into contiguous chunks — efficient for range queries on the shard key, but risks hotspotting if writes cluster around similar/sequential key values (like an auto-incrementing ID). Hashed sharding distributes documents based on a hash of the shard key value, spreading writes very evenly, but making range queries on that field less efficient since similar values end up scattered across shards.

<a id="what-is-a-chunk-in-a-sharded-cluster"></a>
### Q: What is a chunk in a sharded cluster?
**Answer:** A contiguous range of shard key values, and the basic unit MongoDB uses to distribute and balance data across shards. When a chunk grows too large, MongoDB automatically splits it; the balancer then migrates chunks between shards to keep data distributed evenly.

<a id="what-is-the-balancer-and-what-does-it-do"></a>
### Q: What is the balancer, and what does it do?
**Answer:** A background process that monitors the distribution of chunks across shards and automatically migrates them between shards as needed to keep the amount of data on each shard roughly even, preventing any single shard from becoming overloaded relative to the others.

<a id="can-you-change-a-collections-shard-key-after-sharding-it"></a>
### Q: Can you change a collection's shard key after sharding it?
**Answer:** Historically it was effectively fixed at sharding time and very difficult to change without significant manual work (dumping/reloading data). More recent MongoDB versions have introduced the ability to reshard a collection with a new shard key, though it's still a significant, resource-intensive operation that requires careful planning.

<a id="what-is-a-jumbo-chunk-and-why-is-it-a-problem"></a>
### Q: What is a jumbo chunk, and why is it a problem?
**Answer:** A chunk that has grown too large to be split further, often because too many documents share the exact same shard key value, and consequently can't be moved or rebalanced normally by the balancer — a strong sign the chosen shard key doesn't have enough distinct, evenly-distributed values (low cardinality).

---

<a id="transactions-consistency"></a>
## Transactions & Consistency

<a id="are-single-document-writes-in-mongodb-atomic-even-without-an-explicit-transaction"></a>
### Q: Are single-document writes in MongoDB atomic even without an explicit transaction?
**Answer:** Yes — a write to a single document, including updates to multiple fields or nested arrays within that one document, is always atomic by default, with no special transaction needed. Explicit multi-document transactions are only necessary when you need atomicity ACROSS multiple documents or collections in one logical operation.

<a id="what-isolation-guarantees-do-mongodb-transactions-provide"></a>
### Q: What isolation guarantees do MongoDB transactions provide?
**Answer:** Multi-document transactions in MongoDB provide snapshot isolation — all reads within a transaction see a consistent snapshot of data as of the transaction's start, and writes are only visible to other operations once the transaction commits, similar in spirit to "repeatable read" isolation in relational databases.

<a id="what-are-some-downsides-or-limitations-of-using-multi-document-transactions-in-mongodb"></a>
### Q: What are some downsides or limitations of using multi-document transactions in MongoDB?
**Answer:** They add performance overhead compared to atomic single-document writes, have a default execution time limit, can increase lock contention/retries under high concurrency, and are best reserved for cases that genuinely need cross-document atomicity rather than used as a default habit for every write.

<a id="what-is-causal-consistency-in-mongodb"></a>
### Q: What is causal consistency in MongoDB?
**Answer:** A session-level guarantee ensuring that a sequence of read/write operations within the same client session respect their actual cause-and-effect order — e.g. a read after a write in the same causally-consistent session is guaranteed to see that write's effects, even when reading from a different replica set member.

<a id="what-does-read-your-own-writes-mean-in-the-context-of-mongodb-reads"></a>
### Q: What does "read your own writes" mean in the context of MongoDB reads?
**Answer:** A consistency guarantee where a client is assured to see the effects of its own previous write in any subsequent read, within the same session — important when using non-primary read preferences, where without this guarantee a read could otherwise be routed to a secondary that hasn't yet replicated that write.

<a id="what-is-a-write-concern-of-w-0-and-when-if-ever-would-you-use-it"></a>
### Q: What is a write concern of `w: 0`, and when (if ever) would you use it?
**Answer:** `w: 0` means the client doesn't wait for any acknowledgment from the server at all, firing off the write and moving on immediately — the fastest option, but offers no confirmation the write actually succeeded or was even received. Rarely appropriate outside of non-critical, high-throughput logging scenarios where occasional data loss is acceptable.

<a id="what-is-a-retryable-write-and-why-is-it-useful"></a>
### Q: What is a retryable write, and why is it useful?
**Answer:** A feature that lets the MongoDB driver automatically retry certain write operations once if they fail due to a transient network error or replica set failover, without the application needing to manually implement its own retry logic for these common, recoverable failure cases.

<a id="what-is-the-difference-between-optimistic-and-pessimistic-concurrency-control-and-which-does-mongodb-favor"></a>
### Q: What is the difference between optimistic and pessimistic concurrency control, and which does MongoDB favor?
**Answer:** Pessimistic concurrency locks data upfront to prevent conflicting concurrent changes. Optimistic concurrency instead allows concurrent changes and detects conflicts after the fact, e.g. checking a version field before applying an update. MongoDB's document-level atomic operations combined with application-level patterns like a version field checked in the update filter generally favor an optimistic approach for most use cases, rather than heavy explicit locking.

---

<a id="security"></a>
## Security

<a id="how-do-you-enable-authentication-in-mongodb"></a>
### Q: How do you enable authentication in MongoDB?
**Answer:** Enable access control in the server's configuration (`security.authorization: enabled`, or `--auth` at startup), and create at least one administrative user with appropriate roles before restarting with authentication turned on — after which every client connection must authenticate with valid credentials.

<a id="what-is-role-based-access-control-rbac-in-mongodb"></a>
### Q: What is Role-Based Access Control (RBAC) in MongoDB?
**Answer:** A security model where permissions are granted to roles — built-in ones like `read`, `readWrite`, `dbAdmin`, or custom-defined roles — rather than directly to individual users, and users are then assigned one or more roles, simplifying permission management across many users with similar access needs.

<a id="how-do-you-secure-data-at-rest-in-mongodb"></a>
### Q: How do you secure data at rest in MongoDB?
**Answer:** Enable the WiredTiger storage engine's built-in encryption-at-rest feature (available in MongoDB Enterprise/Atlas), which encrypts data files on disk using a configured key management system — protecting data even if the underlying disk/storage media itself is compromised or stolen.

<a id="what-is-the-difference-between-authentication-and-authorization"></a>
### Q: What is the difference between authentication and authorization?
**Answer:** Authentication verifies WHO a client is, validating credentials like username/password, a certificate, or an external identity provider. Authorization determines WHAT that authenticated client is actually allowed to do — which databases/collections/operations they can access — typically governed by their assigned roles.

<a id="what-mechanisms-does-mongodb-support-for-encrypting-data-in-transit"></a>
### Q: What mechanisms does MongoDB support for encrypting data in transit?
**Answer:** TLS/SSL encrypts the connection between clients and the MongoDB server (and between cluster members themselves), preventing eavesdropping or tampering with data as it travels over the network — generally considered essential for any production deployment, especially over the public internet.

<a id="what-is-field-level-encryption-in-mongodb"></a>
### Q: What is field-level encryption in MongoDB?
**Answer:** A feature (Client-Side Field Level Encryption) that encrypts specific sensitive fields on the CLIENT side before they're ever sent to the server, so the data is stored encrypted in the database and even database administrators with direct data access can't read the plaintext value without the corresponding encryption key.

<a id="what-is-ip-whitelisting-and-why-is-it-a-recommended-security-practice-for-mongodb"></a>
### Q: What is IP whitelisting, and why is it a recommended security practice for MongoDB?
**Answer:** Restricting which IP addresses/network ranges are allowed to even attempt a connection to the database server, at the network/firewall level — reducing the attack surface significantly, since unauthorized sources can't reach the server at all, regardless of whether they have valid credentials.

<a id="what-is-the-principle-of-least-privilege-and-how-does-it-apply-to-mongodb-user-roles"></a>
### Q: What is the principle of least privilege, and how does it apply to MongoDB user roles?
**Answer:** Granting each user or application only the minimum permissions actually needed for their function — e.g. an application's regular database user should typically have `readWrite` on only the specific database(s) it needs, not broad admin privileges — limiting the potential damage if that particular credential is ever compromised.

---

<a id="performance-monitoring"></a>
## Performance & Monitoring

<a id="what-is-the-database-profiler-and-how-do-you-use-it"></a>
### Q: What is the Database Profiler, and how do you use it?
**Answer:** A built-in tool that logs detailed information about database operations — queries, writes, commands — that exceed a configurable slow-operation threshold, storing them in a special `system.profile` collection for later analysis. Invaluable for identifying which specific operations are actually causing performance problems in production.

<a id="what-are-common-causes-of-mongodb-performance-bottlenecks"></a>
### Q: What are common causes of MongoDB performance bottlenecks?
**Answer:** Missing or poorly designed indexes forcing full collection scans, a working set that doesn't fit in available RAM (causing excessive disk I/O), an inefficient shard key causing uneven load, overly large documents, and un-optimized aggregation pipelines that don't filter early enough in the sequence of stages.

<a id="what-is-the-working-set-and-why-does-it-matter-for-performance"></a>
### Q: What is the "working set," and why does it matter for performance?
**Answer:** The subset of data (and indexes) actively being accessed by the application on a regular basis. Performance is generally excellent when the working set fits entirely in RAM, so reads are served from memory, but degrades significantly once it exceeds available memory and the server must repeatedly read from disk.

<a id="how-would-you-monitor-a-mongodb-deployment-in-production"></a>
### Q: How would you monitor a MongoDB deployment in production?
**Answer:** Track key metrics like operation latency, queries-per-second, replication lag, connection counts, cache/memory utilization, and disk I/O — using MongoDB's own tools (like `mongostat`/`mongotop`, or the Atlas monitoring dashboard) or third-party integrations (Datadog, Prometheus exporters) that alert on abnormal thresholds.

<a id="what-is-mongostat-and-what-does-it-show"></a>
### Q: What is `mongostat`, and what does it show?
**Answer:** A command-line tool that provides a live, continuously-updating snapshot of a running `mongod`/`mongos` instance's key statistics — operations per second (inserts, queries, updates), memory usage, connections, and replication status — useful for a quick real-time health check.

<a id="what-is-index-cardinality-and-why-does-it-matter-for-query-performance"></a>
### Q: What is index cardinality, and why does it matter for query performance?
**Answer:** Cardinality refers to how many distinct values a field has. High-cardinality fields (like an email address) make for much more selective, efficient indexes, since a query on that field can quickly narrow down to a small set of matching documents — low-cardinality fields (like a boolean) are far less effective as index candidates on their own.

<a id="what-is-connection-pooling-and-why-is-it-important-for-mongodb-clients"></a>
### Q: What is connection pooling, and why is it important for MongoDB clients?
**Answer:** Reusing a pool of established database connections across multiple operations instead of opening and closing a new connection for every single request — since establishing a new connection has real overhead (network handshake, authentication), pooling significantly improves throughput and reduces latency under load.

<a id="how-would-you-identify-and-fix-an-inefficient-query-in-a-live-production-system"></a>
### Q: How would you identify and fix an inefficient query in a live production system?
**Answer:** Enable the profiler (or check slow query logs) to identify specific slow operations, run `.explain("executionStats")` on the offending query to see whether it's using an appropriate index, add or adjust indexes as needed, and re-verify with `explain()` again that the query plan actually improved before considering the fix complete.

---

<a id="common-coding-challenges"></a>
## Common Coding Challenges

<a id="write-an-aggregation-query-to-find-total-sales-per-category"></a>
### Q: Write an aggregation query to find total sales per category.
**Answer:** Group documents by category and sum the amount field across each group, then sort by total descending.

**Example:**
```js
db.sales.aggregate([
  { $group: { _id: '$category', totalSales: { $sum: '$amount' } } },
  { $sort: { totalSales: -1 } },
]);
```

<a id="implement-simple-pagination-using-skip-and-limit"></a>
### Q: Implement simple pagination using `skip()` and `limit()`.
**Answer:** Compute how many documents to skip based on the requested page number and page size, then limit the result to one page's worth.

**Example:**
```js
const pageSize = 10;
const pageNumber = 2;
db.products.find().skip((pageNumber - 1) * pageSize).limit(pageSize);
```

<a id="write-a-query-to-find-the-top-3-highest-paid-employees-in-each-department"></a>
### Q: Write a query to find the top 3 highest-paid employees in each department.
**Answer:** Sort by salary first, group by department while collecting employees into an array, then slice each group's array down to the top 3.

**Example:**
```js
db.employees.aggregate([
  { $sort: { salary: -1 } },
  { $group: { _id: '$department', topEmployees: { $push: { name: '$name', salary: '$salary' } } } },
  { $project: { topEmployees: { $slice: ['$topEmployees', 3] } } },
]);
```

<a id="write-a-query-to-find-documents-where-an-array-field-contains-a-specific-value"></a>
### Q: Write a query to find documents where an array field contains a specific value.
**Answer:** MongoDB automatically matches a scalar value against any element of an array field.

**Example:**
```js
db.products.find({ tags: 'electronics' });
// or, explicitly:
db.products.find({ tags: { $in: ['electronics'] } });
```

<a id="write-an-update-that-increments-a-counter-field-and-pushes-a-value-onto-an-array-in-a-single-operation"></a>
### Q: Write an update that increments a counter field and pushes a value onto an array in a single operation.
**Answer:** Combine `$inc` and `$push` in the same update document — both operators apply atomically together in one call.

**Example:**
```js
db.posts.updateOne(
  { _id: postId },
  { $inc: { viewCount: 1 }, $push: { viewLog: new Date() } }
);
```

<a id="write-a-query-using-lookup-to-join-orders-with-their-corresponding-customer-details"></a>
### Q: Write a query using `$lookup` to join orders with their corresponding customer details.
**Answer:** Use `$lookup` to pull in matching customer documents, then `$unwind` since each order matches exactly one customer.

**Example:**
```js
db.orders.aggregate([
  { $lookup: { from: 'customers', localField: 'customerId', foreignField: '_id', as: 'customer' } },
  { $unwind: '$customer' },
]);
```

<a id="write-a-query-to-find-and-remove-duplicate-documents-based-on-a-field-keeping-only-one-copy"></a>
### Q: Write a query to find and remove duplicate documents based on a field, keeping only one copy.
**Answer:** Group by the field to detect duplicates, filter to groups with more than one document, then delete all but the first `_id` in each group.

**Example:**
```js
db.items.aggregate([
  { $group: { _id: '$email', ids: { $push: '$_id' }, count: { $sum: 1 } } },
  { $match: { count: { $gt: 1 } } },
]).forEach(doc => {
  doc.ids.shift(); // keep the first, remove the rest
  db.items.deleteMany({ _id: { $in: doc.ids } });
});
```

<a id="write-a-query-that-performs-a-case-insensitive-search-on-a-text-field"></a>
### Q: Write a query that performs a case-insensitive search on a text field.
**Answer:** Use `$regex` with the `$options: 'i'` flag for case-insensitive matching.

**Example:**
```js
db.users.find({ name: { $regex: '^john', $options: 'i' } });
```

<a id="write-an-aggregation-to-calculate-the-average-order-value-per-month"></a>
### Q: Write an aggregation to calculate the average order value per month.
**Answer:** Group by year and month extracted from a date field, computing the average of the total field within each group.

**Example:**
```js
db.orders.aggregate([
  { $group: {
      _id: { year: { $year: '$createdAt' }, month: { $month: '$createdAt' } },
      avgOrderValue: { $avg: '$total' },
  }},
  { $sort: { '_id.year': 1, '_id.month': 1 } },
]);
```

<a id="write-a-query-to-atomically-find-a-document-update-it-and-return-the-updated-version"></a>
### Q: Write a query to atomically find a document, update it, and return the updated version.
**Answer:** Use `findOneAndUpdate()` with `returnDocument: 'after'` — commonly used to implement atomic auto-incrementing counters.

**Example:**
```js
db.counters.findOneAndUpdate(
  { _id: 'orderId' },
  { $inc: { seq: 1 } },
  { returnDocument: 'after' }
);
```

---

<a id="behavioral-scenario-based-questions"></a>
## Behavioral / Scenario-Based Questions

<a id="how-would-you-migrate-an-existing-relational-sql-database-to-mongodb"></a>
### Q: How would you migrate an existing relational (SQL) database to MongoDB?
**Answer:** Start by analyzing actual application query patterns rather than mechanically copying the relational schema table-for-table. Identify one-to-few relationships that make sense to embed versus one-to-many/many-to-many relationships better kept as references, migrate data with a script (or a purpose-built tool) that reshapes rows into appropriately-structured documents, and validate the new model against real production query patterns before cutting over.

<a id="how-would-you-design-a-schema-for-a-high-write-volume-application-like-an-iot-sensor-logging-system"></a>
### Q: How would you design a schema for a high-write-volume application, like an IoT sensor logging system?
**Answer:** Favor the Bucket Pattern — grouping many readings into fewer, larger documents (e.g. one document per device per hour) instead of one document per individual reading — to reduce document/index overhead, and choose a shard key (if sharding) that distributes writes evenly rather than clustering around a single hot device or a monotonically increasing timestamp.

<a id="a-collections-queries-are-slow-despite-having-what-looks-like-a-reasonable-index-how-would-you-investigate"></a>
### Q: A collection's queries are slow despite having what looks like a reasonable index — how would you investigate?
**Answer:** Run `.explain("executionStats")` to confirm the index is actually being used as expected and not silently falling back to a collection scan, check whether the query's filter/sort fields actually match the index's field order (especially for compound indexes), verify the working set fits in memory, and check for index selectivity issues if the indexed field has low cardinality.

<a id="how-would-you-handle-a-scenario-where-a-shard-key-choice-turns-out-to-be-causing-uneven-load-across-shards"></a>
### Q: How would you handle a scenario where a shard key choice turns out to be causing uneven load across shards?
**Answer:** Confirm the imbalance with cluster metrics, checking chunk distribution and per-shard operation counts, and depending on MongoDB version, either plan a resharding operation with a better-distributed key, or mitigate at the application level (like adding a hashed suffix to a naturally sequential key) if a full reshard isn't immediately feasible.

<a id="how-would-you-approach-designing-a-mongodb-schema-for-a-social-media-applications-posts-and-comments"></a>
### Q: How would you approach designing a MongoDB schema for a social media application's posts and comments?
**Answer:** It depends on expected comment volume. For posts with typically few comments, embedding a bounded/recent subset directly on the post document (the Subset Pattern) keeps common reads fast. For posts that could accumulate very large numbers of comments over time, comments should be a separate referenced collection to avoid hitting the document size limit and to keep the parent post document lean.

<a id="how-would-you-ensure-data-consistency-when-updating-related-data-across-two-collections-given-mongodb-doesnt-enforce-foreign-key-constraints"></a>
### Q: How would you ensure data consistency when updating related data across two collections, given MongoDB doesn't enforce foreign key constraints?
**Answer:** Use a multi-document transaction if strict atomicity across both collections is required, or carefully design application logic and idempotent operations that gracefully handle partial failure if transactions add too much overhead for the use case — and add safeguards, like periodic consistency-check jobs, to catch and correct any drift between related collections over time.

<a id="how-would-you-approach-capacity-planning-before-sharding-a-growing-mongodb-deployment"></a>
### Q: How would you approach capacity planning before sharding a growing MongoDB deployment?
**Answer:** Analyze current and projected data growth and query/write throughput against the existing unsharded deployment's resource limits, identify a shard key candidate with good cardinality and even distribution matching real access patterns, and test the sharding plan in a staging environment with production-like data volume and load before rolling it out.

<a id="how-would-you-approach-reviewing-a-teammates-proposed-mongodb-schema-in-a-design-review"></a>
### Q: How would you approach reviewing a teammate's proposed MongoDB schema in a design review?
**Answer:** Check that the embed-vs-reference decisions match actual, real application read/write patterns rather than habit, look for unbounded arrays that could eventually exceed the document size limit, verify planned indexes actually support the intended queries, check whether any fields need schema validation rules, and confirm the design accounts for how the data will evolve as the application grows.

---

<a id="how-to-use-this-guide"></a>
## How to Use This Guide

- **A few days before an interview?** Go section by section, top to bottom — each one builds on the last, from basics to sharding and architecture.
- **Revising the night before?** Jump straight to 🔥 Most Asked / Tricky Questions, then skim section headers for anything you're unsure about.
- **During quick revision:** Use `Ctrl+F` (or `Cmd+F`) to jump straight to a keyword or topic instead of scrolling.
- **After every interview:** Come back and add any question you got asked that isn't already here — this file is meant to grow with you.

Good luck — you've got this. 🚀
