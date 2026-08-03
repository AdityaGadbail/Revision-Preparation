# DBMS Interview Questions & Answers — Complete Revision Guide

A complete, structured collection of Database Management Systems interview questions — from fundamentals and ER modeling to normalization, transactions, concurrency control, indexing, and distributed databases — with clear answers and examples where they help. Built to be your one-stop revision resource for interviews, exams, and campus placements.

## 📚 Table of Contents

- [🔥 Most Asked / Tricky Questions](#most-asked-tricky-questions)
  - [What is a DBMS, and how does it differ from a file system?](#what-is-a-dbms-and-how-does-it-differ-from-a-file-system)
  - [What is the difference between DBMS and RDBMS?](#what-is-the-difference-between-dbms-and-rdbms)
  - [What are the three levels of data abstraction (schema architecture) in a DBMS?](#what-are-the-three-levels-of-data-abstraction-schema-architecture-in-a-dbms)
  - [What is data independence, and what are its two types?](#what-is-data-independence-and-what-are-its-two-types)
  - [What is normalization, and what are the main normal forms?](#what-is-normalization-and-what-are-the-main-normal-forms)
  - [What are ACID properties, and why do they matter?](#what-are-acid-properties-and-why-do-they-matter)
  - [What is the difference between a primary key, candidate key, and super key?](#what-is-the-difference-between-a-primary-key-candidate-key-and-super-key)
  - [What is a deadlock, and what are the necessary conditions for one to occur?](#what-is-a-deadlock-and-what-are-the-necessary-conditions-for-one-to-occur)
  - [What is the difference between two-phase locking (2PL) and strict two-phase locking?](#what-is-the-difference-between-two-phase-locking-2pl-and-strict-two-phase-locking)
  - [What is the difference between a clustered index and a non-clustered index?](#what-is-the-difference-between-a-clustered-index-and-a-non-clustered-index)
  - [What is the difference between conflict serializability and view serializability?](#what-is-the-difference-between-conflict-serializability-and-view-serializability)
  - [What is a transaction log (write-ahead log), and why is it needed for recovery?](#what-is-a-transaction-log-write-ahead-log-and-why-is-it-needed-for-recovery)
  - [What is the difference between shared (S) and exclusive (X) locks?](#what-is-the-difference-between-shared-s-and-exclusive-x-locks)
  - [What is the difference between a weak entity and a strong entity in ER modeling?](#what-is-the-difference-between-a-weak-entity-and-a-strong-entity-in-er-modeling)
  - [What is the difference between OLTP and OLAP systems?](#what-is-the-difference-between-oltp-and-olap-systems)
- [DBMS Basics & Architecture](#dbms-basics-architecture)
  - [What are the advantages of using a DBMS over traditional file-based systems?](#what-are-the-advantages-of-using-a-dbms-over-traditional-file-based-systems)
  - [What is a database schema, and how does it differ from a database instance?](#what-is-a-database-schema-and-how-does-it-differ-from-a-database-instance)
  - [What is a Database Administrator (DBA), and what are typical responsibilities?](#what-is-a-database-administrator-dba-and-what-are-typical-responsibilities)
  - [What are the main components of a DBMS architecture?](#what-are-the-main-components-of-a-dbms-architecture)
  - [What is the difference between a 2-tier and 3-tier database architecture?](#what-is-the-difference-between-a-2-tier-and-3-tier-database-architecture)
  - [What is a data dictionary (system catalog)?](#what-is-a-data-dictionary-system-catalog)
  - [What are the different data models used in database systems?](#what-are-the-different-data-models-used-in-database-systems)
  - [What is the difference between a database and a data warehouse?](#what-is-the-difference-between-a-database-and-a-data-warehouse)
  - [What is metadata in the context of a database?](#what-is-metadata-in-the-context-of-a-database)
  - [What is the difference between DDL, DML, and DCL commands?](#what-is-the-difference-between-ddl-dml-and-dcl-commands)
  - [What is data redundancy, and why is it problematic?](#what-is-data-redundancy-and-why-is-it-problematic)
  - [What is the difference between a centralized and a distributed database?](#what-is-the-difference-between-a-centralized-and-a-distributed-database)
- [ER Model & Data Modeling](#er-model-data-modeling)
  - [What is an Entity-Relationship (ER) diagram, and what is it used for?](#what-is-an-entity-relationship-er-diagram-and-what-is-it-used-for)
  - [What is the difference between an entity and an entity set?](#what-is-the-difference-between-an-entity-and-an-entity-set)
  - [What are the different types of attributes in ER modeling?](#what-are-the-different-types-of-attributes-in-er-modeling)
  - [What is the difference between a weak entity and a strong entity?](#what-is-the-difference-between-a-weak-entity-and-a-strong-entity)
  - [What are the different types of relationship cardinality?](#what-are-the-different-types-of-relationship-cardinality)
  - [What is total vs. partial participation in ER modeling?](#what-is-total-vs-partial-participation-in-er-modeling)
  - [How is a many-to-many relationship implemented in a relational database?](#how-is-a-many-to-many-relationship-implemented-in-a-relational-database)
  - [What is generalization and specialization in ER modeling?](#what-is-generalization-and-specialization-in-er-modeling)
  - [What is aggregation in ER modeling?](#what-is-aggregation-in-er-modeling)
  - [How do you convert an ER diagram into relational tables?](#how-do-you-convert-an-er-diagram-into-relational-tables)
- [Relational Model & Keys](#relational-model-keys)
  - [What is the relational model, and who introduced it?](#what-is-the-relational-model-and-who-introduced-it)
  - [What is a tuple, and what is a relation, in relational model terminology?](#what-is-a-tuple-and-what-is-a-relation-in-relational-model-terminology)
  - [What is the difference between a candidate key, primary key, and alternate key?](#what-is-the-difference-between-a-candidate-key-primary-key-and-alternate-key)
  - [What is a composite key?](#what-is-a-composite-key)
  - [What is a foreign key, and what does it enforce?](#what-is-a-foreign-key-and-what-does-it-enforce)
  - [What is entity integrity, and what does it require?](#what-is-entity-integrity-and-what-does-it-require)
  - [What is referential integrity?](#what-is-referential-integrity)
  - [What is a surrogate key, and how does it differ from a natural key?](#what-is-a-surrogate-key-and-how-does-it-differ-from-a-natural-key)
  - [What is a relational schema, and what is a relational instance?](#what-is-a-relational-schema-and-what-is-a-relational-instance)
  - [What are integrity constraints in a relational database, and name common types?](#what-are-integrity-constraints-in-a-relational-database-and-name-common-types)
- [Normalization & Functional Dependencies](#normalization-functional-dependencies)
  - [What is a functional dependency?](#what-is-a-functional-dependency)
  - [What is a partial dependency?](#what-is-a-partial-dependency)
  - [What is a transitive dependency?](#what-is-a-transitive-dependency)
  - [What is First Normal Form (1NF)?](#what-is-first-normal-form-1nf)
  - [What is Second Normal Form (2NF)?](#what-is-second-normal-form-2nf)
  - [What is Third Normal Form (3NF)?](#what-is-third-normal-form-3nf)
  - [What is Boyce-Codd Normal Form (BCNF), and how does it differ from 3NF?](#what-is-boyce-codd-normal-form-bcnf-and-how-does-it-differ-from-3nf)
  - [What is a multivalued dependency, and what normal form addresses it?](#what-is-a-multivalued-dependency-and-what-normal-form-addresses-it)
  - [What is denormalization, and when might you intentionally use it?](#what-is-denormalization-and-when-might-you-intentionally-use-it)
  - [What are Armstrong's Axioms, and why are they important for functional dependencies?](#what-are-armstrongs-axioms-and-why-are-they-important-for-functional-dependencies)
- [SQL & Relational Algebra](#sql-relational-algebra)
  - [What is relational algebra, and what is its role in a DBMS?](#what-is-relational-algebra-and-what-is-its-role-in-a-dbms)
  - [What is the difference between the selection and projection operations in relational algebra?](#what-is-the-difference-between-the-selection-and-projection-operations-in-relational-algebra)
  - [What is the difference between the union, intersection, and set difference operations in relational algebra?](#what-is-the-difference-between-the-union-intersection-and-set-difference-operations-in-relational-algebra)
  - [What is a natural join in relational algebra, and how does it relate to SQL's `JOIN`?](#what-is-a-natural-join-in-relational-algebra-and-how-does-it-relate-to-sqls-join)
  - [What is the Cartesian product operation, and how does it relate to a `CROSS JOIN`?](#what-is-the-cartesian-product-operation-and-how-does-it-relate-to-a-cross-join)
  - [What is the difference between DDL, DML, DQL, DCL, and TCL SQL command categories?](#what-is-the-difference-between-ddl-dml-dql-dcl-and-tcl-sql-command-categories)
  - [What is a view in relational database terms, and what relational algebra concept does it correspond to?](#what-is-a-view-in-relational-database-terms-and-what-relational-algebra-concept-does-it-correspond-to)
  - [What is the difference between tuple relational calculus and domain relational calculus?](#what-is-the-difference-between-tuple-relational-calculus-and-domain-relational-calculus)
  - [How does a query optimizer use relational algebra internally when processing a SQL query?](#how-does-a-query-optimizer-use-relational-algebra-internally-when-processing-a-sql-query)
  - [What is the difference between a scalar subquery and using a `JOIN` to achieve the same result?](#what-is-the-difference-between-a-scalar-subquery-and-using-a-join-to-achieve-the-same-result)
- [Transactions & Concurrency Control](#transactions-concurrency-control)
  - [What is a transaction, and what are its typical states?](#what-is-a-transaction-and-what-are-its-typical-states)
  - [What is the difference between a schedule and a serial schedule?](#what-is-the-difference-between-a-schedule-and-a-serial-schedule)
  - [What is serializability, and why does it matter?](#what-is-serializability-and-why-does-it-matter)
  - [What is the difference between conflict serializability and view serializability?](#what-is-the-difference-between-conflict-serializability-and-view-serializability-2)
  - [What is two-phase locking (2PL), and what are its two phases?](#what-is-two-phase-locking-2pl-and-what-are-its-two-phases)
  - [What is the difference between 2PL, strict 2PL, and rigorous 2PL?](#what-is-the-difference-between-2pl-strict-2pl-and-rigorous-2pl)
  - [What is timestamp ordering, and how does it differ from lock-based concurrency control?](#what-is-timestamp-ordering-and-how-does-it-differ-from-lock-based-concurrency-control)
  - [What is optimistic concurrency control, and how does it differ from pessimistic approaches?](#what-is-optimistic-concurrency-control-and-how-does-it-differ-from-pessimistic-approaches)
  - [What is a cascading rollback, and how do stricter locking protocols prevent it?](#what-is-a-cascading-rollback-and-how-do-stricter-locking-protocols-prevent-it)
  - [What is the difference between recoverable and non-recoverable schedules?](#what-is-the-difference-between-recoverable-and-non-recoverable-schedules)
  - [What is multi-version concurrency control (MVCC), and what problem does it solve?](#what-is-multi-version-concurrency-control-mvcc-and-what-problem-does-it-solve)
  - [What is lock granularity, and what is multiple granularity locking?](#what-is-lock-granularity-and-what-is-multiple-granularity-locking)
- [Indexing & File Organization](#indexing-file-organization)
  - [What is indexing in a DBMS, and why is it used?](#what-is-indexing-in-a-dbms-and-why-is-it-used)
  - [What is the difference between a primary index, secondary index, and clustering index?](#what-is-the-difference-between-a-primary-index-secondary-index-and-clustering-index)
  - [What is a dense index vs. a sparse index?](#what-is-a-dense-index-vs-a-sparse-index)
  - [What is a B-tree, and why is it commonly used for database indexes?](#what-is-a-b-tree-and-why-is-it-commonly-used-for-database-indexes)
  - [What is the difference between a B-tree and a B+ tree?](#what-is-the-difference-between-a-b-tree-and-a-b-tree)
  - [What is hashing, and how does hash-based indexing differ from B-tree indexing?](#what-is-hashing-and-how-does-hash-based-indexing-differ-from-b-tree-indexing)
  - [What is the difference between static hashing and dynamic hashing?](#what-is-the-difference-between-static-hashing-and-dynamic-hashing)
  - [What is file organization, and what are the common types?](#what-is-file-organization-and-what-are-the-common-types)
  - [What is a composite index, and how does column order affect its usefulness?](#what-is-a-composite-index-and-how-does-column-order-affect-its-usefulness)
  - [What is the trade-off between having more indexes on a table?](#what-is-the-trade-off-between-having-more-indexes-on-a-table)
- [Deadlocks & Recovery](#deadlocks-recovery)
  - [What are the four necessary conditions for a deadlock?](#what-are-the-four-necessary-conditions-for-a-deadlock)
  - [What is the difference between deadlock prevention, avoidance, and detection?](#what-is-the-difference-between-deadlock-prevention-avoidance-and-detection)
  - [What is a wait-for graph, and how is it used to detect deadlocks?](#what-is-a-wait-for-graph-and-how-is-it-used-to-detect-deadlocks)
  - [What is the difference between the wait-die and wound-wait deadlock prevention schemes?](#what-is-the-difference-between-the-wait-die-and-wound-wait-deadlock-prevention-schemes)
  - [What is a checkpoint, and why is it used in database recovery?](#what-is-a-checkpoint-and-why-is-it-used-in-database-recovery)
  - [What is the difference between the redo and undo phases of database recovery?](#what-is-the-difference-between-the-redo-and-undo-phases-of-database-recovery)
  - [What is shadow paging, and how does it differ from log-based recovery?](#what-is-shadow-paging-and-how-does-it-differ-from-log-based-recovery)
  - [What is the write-ahead logging (WAL) rule, and why is it fundamental to crash recovery?](#what-is-the-write-ahead-logging-wal-rule-and-why-is-it-fundamental-to-crash-recovery)
- [Distributed Databases & NoSQL](#distributed-databases-nosql)
  - [What is a distributed database, and what are its main advantages?](#what-is-a-distributed-database-and-what-are-its-main-advantages)
  - [What is data fragmentation in a distributed database, and what are its types?](#what-is-data-fragmentation-in-a-distributed-database-and-what-are-its-types)
  - [What is the CAP theorem, and what does it state?](#what-is-the-cap-theorem-and-what-does-it-state)
  - [What is eventual consistency, and where is it commonly used?](#what-is-eventual-consistency-and-where-is-it-commonly-used)
  - [What is the difference between a distributed database and a NoSQL database?](#what-is-the-difference-between-a-distributed-database-and-a-nosql-database)
  - [What are the main categories of NoSQL databases?](#what-are-the-main-categories-of-nosql-databases)
  - [What is a two-phase commit protocol, and what problem does it solve in distributed transactions?](#what-is-a-two-phase-commit-protocol-and-what-problem-does-it-solve-in-distributed-transactions)
  - [What is data replication in a distributed database, and what are its trade-offs?](#what-is-data-replication-in-a-distributed-database-and-what-are-its-trade-offs)
- [Database Security](#database-security)
  - [What is database security, and why is it important?](#what-is-database-security-and-why-is-it-important)
  - [What is the difference between authentication and authorization in database security?](#what-is-the-difference-between-authentication-and-authorization-in-database-security)
  - [What is SQL injection, and how do you prevent it?](#what-is-sql-injection-and-how-do-you-prevent-it)
  - [What is Role-Based Access Control (RBAC), and why is it useful for managing database permissions?](#what-is-role-based-access-control-rbac-and-why-is-it-useful-for-managing-database-permissions)
  - [What is the principle of least privilege, and how does it apply to database access?](#what-is-the-principle-of-least-privilege-and-how-does-it-apply-to-database-access)
  - [What is encryption at rest vs. encryption in transit?](#what-is-encryption-at-rest-vs-encryption-in-transit)
  - [What is database auditing, and why is it used?](#what-is-database-auditing-and-why-is-it-used)
  - [What is data masking, and when would you use it?](#what-is-data-masking-and-when-would-you-use-it)
- [Common Conceptual & Coding Challenges](#common-conceptual-coding-challenges)
  - [Given a relation with a composite primary key, how would you identify whether it's in 2NF?](#given-a-relation-with-a-composite-primary-key-how-would-you-identify-whether-its-in-2nf)
  - [Given a functional dependency set, how would you determine the candidate key(s) of a relation?](#given-a-functional-dependency-set-how-would-you-determine-the-candidate-keys-of-a-relation)
  - [How would you design a schema, in 3NF, for a simple library management system?](#how-would-you-design-a-schema-in-3nf-for-a-simple-library-management-system)
  - [Given a precedence graph for a schedule, how would you determine if it's conflict-serializable?](#given-a-precedence-graph-for-a-schedule-how-would-you-determine-if-its-conflict-serializable)
  - [Given a set of transactions and lock requests, how would you identify whether a deadlock occurs?](#given-a-set-of-transactions-and-lock-requests-how-would-you-identify-whether-a-deadlock-occurs)
  - [How would you compute the number of block accesses needed for a linear search vs. a binary search on a sorted, indexed file?](#how-would-you-compute-the-number-of-block-accesses-needed-for-a-linear-search-vs-a-binary-search-on-a-sorted-indexed-file)
  - [Given a relation, how would you write the relational algebra expression to find rows matching a condition and only certain columns?](#given-a-relation-how-would-you-write-the-relational-algebra-expression-to-find-rows-matching-a-condition-and-only-certain-columns)
  - [Given two relations, how would you write the relational algebra expression for a natural join?](#given-two-relations-how-would-you-write-the-relational-algebra-expression-for-a-natural-join)
  - [How would you determine whether a given database design suffers from an update anomaly?](#how-would-you-determine-whether-a-given-database-design-suffers-from-an-update-anomaly)
  - [Given a scenario with concurrent transactions, what happens if you apply strict two-phase locking?](#given-a-scenario-with-concurrent-transactions-what-happens-if-you-apply-strict-two-phase-locking)
- [Behavioral / Scenario-Based Questions](#behavioral-scenario-based-questions)
  - [How would you approach designing a database schema for a new application from scratch?](#how-would-you-approach-designing-a-database-schema-for-a-new-application-from-scratch)
  - [How would you diagnose and resolve a deadlock occurring in a production system?](#how-would-you-diagnose-and-resolve-a-deadlock-occurring-in-a-production-system)
  - [How would you decide between normalizing fully and selectively denormalizing part of a schema?](#how-would-you-decide-between-normalizing-fully-and-selectively-denormalizing-part-of-a-schema)
  - [How would you explain the trade-off between strong consistency and high availability to a non-technical stakeholder?](#how-would-you-explain-the-trade-off-between-strong-consistency-and-high-availability-to-a-non-technical-stakeholder)
  - [How would you approach recovering a database after a server crash?](#how-would-you-approach-recovering-a-database-after-a-server-crash)
  - [How would you choose between a relational database and a NoSQL database for a new project?](#how-would-you-choose-between-a-relational-database-and-a-nosql-database-for-a-new-project)
  - [How would you investigate a query that's performing much slower than expected in production?](#how-would-you-investigate-a-query-thats-performing-much-slower-than-expected-in-production)
  - [How would you approach reviewing a teammate's proposed database schema in a design review?](#how-would-you-approach-reviewing-a-teammates-proposed-database-schema-in-a-design-review)
- [How to Use This Guide](#how-to-use-this-guide)

---

<a id="most-asked-tricky-questions"></a>
## 🔥 Most Asked / Tricky Questions

These come up in almost every DBMS interview. If you're short on time, start here.

<a id="what-is-a-dbms-and-how-does-it-differ-from-a-file-system"></a>
### Q: What is a DBMS, and how does it differ from a file system?
**Answer:** A DBMS (Database Management System) is software that manages the creation, storage, retrieval, and manipulation of data in a structured way, providing data integrity, concurrent access control, security, and a query interface. A plain file system just stores raw files with no built-in understanding of the data's structure, no enforced integrity/consistency rules, no query language, and much weaker concurrent-access safety — a DBMS solves problems like data redundancy, inconsistency, and difficulty of multi-user access that plain file-based storage suffers from.

<a id="what-is-the-difference-between-dbms-and-rdbms"></a>
### Q: What is the difference between DBMS and RDBMS?
**Answer:** A DBMS is the general category of software for managing databases, without necessarily enforcing a particular data model. An RDBMS specifically organizes data into related tables with rows and columns, enforces relationships through keys, and typically supports SQL along with ACID transactions and normalization — most modern production databases like PostgreSQL, MySQL, and Oracle are RDBMSs.

<a id="what-are-the-three-levels-of-data-abstraction-schema-architecture-in-a-dbms"></a>
### Q: What are the three levels of data abstraction (schema architecture) in a DBMS?
**Answer:** The internal (physical) level describes how data is actually stored on disk. The conceptual (logical) level describes what data is stored and the relationships between it, independent of physical storage details. The external (view) level describes how individual users or applications see a customized subset/presentation of the data. This ANSI/SPARC architecture provides data independence between how data is stored, structured, and consumed.

<a id="what-is-data-independence-and-what-are-its-two-types"></a>
### Q: What is data independence, and what are its two types?
**Answer:** Data independence is the ability to change a schema at one level of the database architecture without requiring changes at the level(s) above it. Logical data independence means changes to the conceptual schema don't require changing external views/application code. Physical data independence means changes to the internal storage don't require changing the conceptual schema.

<a id="what-is-normalization-and-what-are-the-main-normal-forms"></a>
### Q: What is normalization, and what are the main normal forms?
**Answer:** Normalization organizes tables to minimize data redundancy and avoid update/insert/delete anomalies, following a series of increasingly strict rules. 1NF requires atomic column values. 2NF requires every non-key attribute to depend on the whole primary key, not just part of it. 3NF requires no transitive dependencies between non-key attributes. BCNF is a stricter version of 3NF handling certain edge cases with overlapping candidate keys.

<a id="what-are-acid-properties-and-why-do-they-matter"></a>
### Q: What are ACID properties, and why do they matter?
**Answer:** Atomicity (a transaction is all-or-nothing), Consistency (a transaction takes the database from one valid state to another, respecting all constraints), Isolation (concurrent transactions don't interfere with or see each other's uncommitted changes), and Durability (once committed, changes survive even a system crash). Together they guarantee reliable, predictable behavior even under concurrent access and failures.

<a id="what-is-the-difference-between-a-primary-key-candidate-key-and-super-key"></a>
### Q: What is the difference between a primary key, candidate key, and super key?
**Answer:** A super key is any set of attributes that can uniquely identify a row, possibly with redundant extra attributes. A candidate key is a minimal super key — no attribute can be removed without losing uniqueness. A primary key is the one candidate key specifically chosen as the table's main unique identifier; other candidate keys not chosen become alternate keys.

<a id="what-is-a-deadlock-and-what-are-the-necessary-conditions-for-one-to-occur"></a>
### Q: What is a deadlock, and what are the necessary conditions for one to occur?
**Answer:** A deadlock is a situation where two or more transactions are each waiting for a lock the other holds, so none can proceed. Four necessary conditions must all hold: mutual exclusion (resources can't be shared), hold and wait (a transaction holds a resource while waiting for another), no preemption (resources can't be forcibly taken away), and circular wait (a cycle of transactions each waiting on the next).

<a id="what-is-the-difference-between-two-phase-locking-2pl-and-strict-two-phase-locking"></a>
### Q: What is the difference between two-phase locking (2PL) and strict two-phase locking?
**Answer:** In 2PL, a transaction has a growing phase, acquiring locks and never releasing any, followed by a shrinking phase, releasing locks and never acquiring more — this guarantees serializability but can still allow cascading rollbacks. Strict 2PL additionally holds all exclusive (write) locks until the transaction actually commits or aborts, preventing other transactions from ever reading uncommitted data and thus avoiding cascading rollbacks entirely.

<a id="what-is-the-difference-between-a-clustered-index-and-a-non-clustered-index"></a>
### Q: What is the difference between a clustered index and a non-clustered index?
**Answer:** A clustered index determines the actual physical order rows are stored on disk — a table can have only one, since data can only be physically sorted one way. A non-clustered index is a separate structure holding sorted key values with pointers back to the actual row location, and a table can have several of them.

<a id="what-is-the-difference-between-conflict-serializability-and-view-serializability"></a>
### Q: What is the difference between conflict serializability and view serializability?
**Answer:** Conflict serializability determines whether a schedule is equivalent to some serial schedule by swapping only non-conflicting operations — checkable efficiently via a precedence graph having no cycles. View serializability is a broader, less strict condition based on whether transactions read the same values and produce the same final writes as some serial order — every conflict-serializable schedule is view-serializable, but not vice versa, and it's much harder to test efficiently.

<a id="what-is-a-transaction-log-write-ahead-log-and-why-is-it-needed-for-recovery"></a>
### Q: What is a transaction log (write-ahead log), and why is it needed for recovery?
**Answer:** A transaction log records every change made to the database, often before the change is even applied to the actual data files, so that after a crash the database can be restored to a consistent state — redoing committed transactions not yet fully flushed to disk, and undoing uncommitted transactions in progress at the time of the crash.

<a id="what-is-the-difference-between-shared-s-and-exclusive-x-locks"></a>
### Q: What is the difference between shared (S) and exclusive (X) locks?
**Answer:** A shared lock allows multiple transactions to simultaneously read the same data item, but prevents any of them from writing to it. An exclusive lock allows only one transaction to hold it at a time, needed for writing, and is incompatible with both other exclusive locks and any shared locks on the same data.

<a id="what-is-the-difference-between-a-weak-entity-and-a-strong-entity-in-er-modeling"></a>
### Q: What is the difference between a weak entity and a strong entity in ER modeling?
**Answer:** A strong entity has its own primary key and can exist independently. A weak entity lacks a sufficient set of attributes to form its own primary key, and depends on a relationship with a strong owner entity — its partial key combined with the owner entity's primary key together form its actual identifying key.

<a id="what-is-the-difference-between-oltp-and-olap-systems"></a>
### Q: What is the difference between OLTP and OLAP systems?
**Answer:** OLTP (Online Transaction Processing) systems handle frequent, short, simple read/write transactions, like processing individual orders, optimized for fast concurrent updates. OLAP (Online Analytical Processing) systems handle complex, read-heavy analytical queries over large historical datasets, typically using denormalized, aggregated data structures optimized for scanning and summarizing rather than fast individual updates.

---

<a id="dbms-basics-architecture"></a>
## DBMS Basics & Architecture

<a id="what-are-the-advantages-of-using-a-dbms-over-traditional-file-based-systems"></a>
### Q: What are the advantages of using a DBMS over traditional file-based systems?
**Answer:** Reduced data redundancy and inconsistency, controlled and secure concurrent access by multiple users, data integrity enforced through constraints, a standardized query interface instead of custom file-parsing code, backup/recovery support, and easier enforcement of data independence as the application evolves.

<a id="what-is-a-database-schema-and-how-does-it-differ-from-a-database-instance"></a>
### Q: What is a database schema, and how does it differ from a database instance?
**Answer:** A schema is the overall logical design/structure of a database — its tables, columns, data types, and relationships — defined once and rarely changed. An instance is the actual data stored in the database at a particular moment in time, constantly changing as data is inserted, updated, or deleted, while the schema usually stays fixed.

<a id="what-is-a-database-administrator-dba-and-what-are-typical-responsibilities"></a>
### Q: What is a Database Administrator (DBA), and what are typical responsibilities?
**Answer:** A DBA manages a database system's day-to-day operation and health — schema design, performance tuning, backup and recovery planning, managing user access/permissions, monitoring for issues, and capacity planning as data grows.

<a id="what-are-the-main-components-of-a-dbms-architecture"></a>
### Q: What are the main components of a DBMS architecture?
**Answer:** The query processor (parses and optimizes queries), the storage manager (handles how data is physically stored and retrieved, including buffer/cache management), the transaction manager (ensures ACID properties), and the metadata/data dictionary (stores the schema and other information about the database itself).

<a id="what-is-the-difference-between-a-2-tier-and-3-tier-database-architecture"></a>
### Q: What is the difference between a 2-tier and 3-tier database architecture?
**Answer:** A 2-tier architecture has the client application communicating directly with the database server. A 3-tier architecture inserts an application/business-logic layer between the client and the database, so the client never talks to the database directly — improving security, scalability, and separation of concerns, common in most modern web applications.

<a id="what-is-a-data-dictionary-system-catalog"></a>
### Q: What is a data dictionary (system catalog)?
**Answer:** A special set of metadata tables the DBMS itself maintains, describing the database's own structure — table and column names, data types, constraints, indexes, and access permissions — used internally to validate and optimize queries, and often queryable by users/admins directly.

<a id="what-are-the-different-data-models-used-in-database-systems"></a>
### Q: What are the different data models used in database systems?
**Answer:** The hierarchical model (tree-structured, parent-child relationships), the network model (a more flexible graph of relationships, generalizing hierarchical), the relational model (tables/rows/columns linked by keys, the dominant model today), and the object-oriented/object-relational model (data represented as objects, blending OOP concepts with database storage).

<a id="what-is-the-difference-between-a-database-and-a-data-warehouse"></a>
### Q: What is the difference between a database and a data warehouse?
**Answer:** A typically OLTP database stores current, frequently-updated operational data supporting an application's day-to-day transactions. A data warehouse stores large volumes of historical data aggregated from multiple sources, structured and optimized specifically for analytical querying and reporting rather than for frequent individual transaction updates.

<a id="what-is-metadata-in-the-context-of-a-database"></a>
### Q: What is metadata in the context of a database?
**Answer:** Data that describes other data — in a database context, this means information about the database's own structure, like table/column names, data types, constraints, and relationships, rather than the actual application data itself.

<a id="what-is-the-difference-between-ddl-dml-and-dcl-commands"></a>
### Q: What is the difference between DDL, DML, and DCL commands?
**Answer:** DDL (`CREATE`, `ALTER`, `DROP`) defines and modifies the database's structure. DML (`SELECT`, `INSERT`, `UPDATE`, `DELETE`) manages the actual data within that structure. DCL (`GRANT`, `REVOKE`) manages user permissions and access control.

<a id="what-is-data-redundancy-and-why-is-it-problematic"></a>
### Q: What is data redundancy, and why is it problematic?
**Answer:** Data redundancy is the same piece of information being stored in multiple places unnecessarily. It's problematic because it wastes storage, and more importantly risks data inconsistency — if the same fact is updated in one location but not the others, the database ends up containing contradictory information.

<a id="what-is-the-difference-between-a-centralized-and-a-distributed-database"></a>
### Q: What is the difference between a centralized and a distributed database?
**Answer:** A centralized database stores all its data on a single server/location, managed by one central DBMS instance. A distributed database spreads data across multiple physical locations/servers, which may be geographically dispersed, appearing to users as a single logical database despite the underlying physical distribution.

---

<a id="er-model-data-modeling"></a>
## ER Model & Data Modeling

<a id="what-is-an-entity-relationship-er-diagram-and-what-is-it-used-for"></a>
### Q: What is an Entity-Relationship (ER) diagram, and what is it used for?
**Answer:** A visual modeling tool representing a database's entities (things being tracked, like Customer or Product), their attributes (properties, like name or price), and the relationships between entities (like a Customer placing an Order) — used during the database design phase, before physical implementation, to plan and communicate the intended structure.

<a id="what-is-the-difference-between-an-entity-and-an-entity-set"></a>
### Q: What is the difference between an entity and an entity set?
**Answer:** An entity is a single, specific instance of a real-world object or concept being represented, like one particular customer. An entity set is the entire collection of similar entities sharing the same attributes, like all Customers — conceptually corresponding to a table once implemented in a relational database.

<a id="what-are-the-different-types-of-attributes-in-er-modeling"></a>
### Q: What are the different types of attributes in ER modeling?
**Answer:** Simple (atomic, can't be divided further, like age), composite (can be broken into sub-parts, like a full name split into first/last), single-valued (one value per entity, like a birthdate), multi-valued (can have several values, like multiple phone numbers), and derived (computed from other attributes, like age derived from a birthdate).

<a id="what-is-the-difference-between-a-weak-entity-and-a-strong-entity"></a>
### Q: What is the difference between a weak entity and a strong entity?
**Answer:** A strong entity has its own primary key and can exist independently. A weak entity lacks a sufficient set of attributes to form its own primary key, and depends on a relationship with an owning strong entity — its partial key combined with the owner's primary key together identify it uniquely.

<a id="what-are-the-different-types-of-relationship-cardinality"></a>
### Q: What are the different types of relationship cardinality?
**Answer:** One-to-one (each entity in set A relates to at most one entity in set B, and vice versa), one-to-many (one entity in A can relate to many in B, but each in B relates to only one in A), and many-to-many (entities in both sets can relate to multiple entities on the other side).

<a id="what-is-total-vs-partial-participation-in-er-modeling"></a>
### Q: What is total vs. partial participation in ER modeling?
**Answer:** Total participation means every entity in a set must participate in a given relationship, e.g. every employee must belong to some department. Partial participation means some entities in the set may not participate in that relationship at all, e.g. not every employee necessarily manages a project.

<a id="how-is-a-many-to-many-relationship-implemented-in-a-relational-database"></a>
### Q: How is a many-to-many relationship implemented in a relational database?
**Answer:** Since a relational table can't directly represent many-to-many relationships on its own, a separate junction (or bridge) table is created, holding foreign keys referencing both related entities' primary keys, typically forming a composite primary key across those two foreign key columns.

<a id="what-is-generalization-and-specialization-in-er-modeling"></a>
### Q: What is generalization and specialization in ER modeling?
**Answer:** Generalization is a bottom-up process combining several entity sets that share common attributes into one broader, more general entity set, e.g. combining Car and Truck into Vehicle. Specialization is the reverse, top-down process, dividing a broader entity set into more specific sub-entity sets with additional distinguishing attributes, e.g. splitting Employee into Manager and Engineer.

<a id="what-is-aggregation-in-er-modeling"></a>
### Q: What is aggregation in ER modeling?
**Answer:** A modeling technique that treats an entire relationship between two entities as if it were itself a higher-level entity, letting that combined relationship participate in further relationships with other entities — used when a relationship itself needs to be related to something else, which basic ER notation can't directly express otherwise.

<a id="how-do-you-convert-an-er-diagram-into-relational-tables"></a>
### Q: How do you convert an ER diagram into relational tables?
**Answer:** Each strong entity set becomes its own table, with its attributes as columns and its identifying attribute as the primary key. Each weak entity set becomes a table that includes the owner entity's primary key as a foreign key, combined with its own partial key, to form its composite primary key. Relationships typically become foreign keys for one-to-many, or entirely separate junction tables for many-to-many.

---

<a id="relational-model-keys"></a>
## Relational Model & Keys

<a id="what-is-the-relational-model-and-who-introduced-it"></a>
### Q: What is the relational model, and who introduced it?
**Answer:** A data model, introduced by E.F. Codd in 1970, that represents data as a collection of relations (tables), each consisting of rows (tuples) and columns (attributes), with relationships between tables expressed through shared key values rather than physical pointers.

<a id="what-is-a-tuple-and-what-is-a-relation-in-relational-model-terminology"></a>
### Q: What is a tuple, and what is a relation, in relational model terminology?
**Answer:** A tuple is a single row of a relation, representing one specific record. A relation is the formal term for what's commonly called a table — a set of tuples all sharing the same structure of attributes.

<a id="what-is-the-difference-between-a-candidate-key-primary-key-and-alternate-key"></a>
### Q: What is the difference between a candidate key, primary key, and alternate key?
**Answer:** A candidate key is any minimal set of attributes that can uniquely identify a tuple. The primary key is the specific candidate key chosen as the table's main identifier. Alternate keys are any remaining candidate keys that weren't chosen as the primary key.

<a id="what-is-a-composite-key"></a>
### Q: What is a composite key?
**Answer:** A key made up of two or more attributes together, where the combination uniquely identifies a tuple, even though no single attribute alone does — common in relationship/junction tables representing many-to-many associations.

<a id="what-is-a-foreign-key-and-what-does-it-enforce"></a>
### Q: What is a foreign key, and what does it enforce?
**Answer:** An attribute (or set of attributes) in one table that references the primary key of another table, establishing a link between them. It enforces referential integrity — you can't insert a row referencing a non-existent parent row in the referenced table.

<a id="what-is-entity-integrity-and-what-does-it-require"></a>
### Q: What is entity integrity, and what does it require?
**Answer:** A constraint requiring that no primary key attribute can contain a `NULL` value — since a primary key's purpose is to uniquely identify each row, allowing `NULL` there would make that guarantee meaningless.

<a id="what-is-referential-integrity"></a>
### Q: What is referential integrity?
**Answer:** A constraint requiring that any foreign key value in a table must either match an existing primary key value in the referenced table, or be `NULL` if the foreign key column allows nulls — preventing orphaned references to rows that don't actually exist.

<a id="what-is-a-surrogate-key-and-how-does-it-differ-from-a-natural-key"></a>
### Q: What is a surrogate key, and how does it differ from a natural key?
**Answer:** A surrogate key is an artificially generated identifier, like an auto-incrementing integer, with no inherent business meaning, used purely to uniquely identify a row. A natural key is derived from actual real-world data that's already unique, like an email address — surrogate keys are generally preferred since natural keys can sometimes change or turn out not to be as unique as assumed.

<a id="what-is-a-relational-schema-and-what-is-a-relational-instance"></a>
### Q: What is a relational schema, and what is a relational instance?
**Answer:** A relational schema describes a relation's structure — its name and the set of attributes with their data types/domains. A relational instance is the actual set of tuples currently populating that relation at a given point in time.

<a id="what-are-integrity-constraints-in-a-relational-database-and-name-common-types"></a>
### Q: What are integrity constraints in a relational database, and name common types?
**Answer:** Rules the DBMS enforces to maintain data accuracy and consistency. Common types: domain constraints (values must come from a valid, defined set/type), entity integrity (primary key can't be `NULL`), referential integrity (foreign keys must reference existing rows), and key constraints (uniqueness requirements).

---

<a id="normalization-functional-dependencies"></a>
## Normalization & Functional Dependencies

<a id="what-is-a-functional-dependency"></a>
### Q: What is a functional dependency?
**Answer:** A constraint between two sets of attributes in a relation, written A → B, meaning that for any two tuples sharing the same value(s) for A, they must also share the same value(s) for B — B's value is fully determined by A's value.

<a id="what-is-a-partial-dependency"></a>
### Q: What is a partial dependency?
**Answer:** A situation where a non-key attribute depends on only part of a composite primary key, rather than the entire key — this specifically violates Second Normal Form (2NF) if it occurs.

<a id="what-is-a-transitive-dependency"></a>
### Q: What is a transitive dependency?
**Answer:** A situation where a non-key attribute depends on another non-key attribute, rather than depending directly on the primary key — e.g. if a zip code determines a city, and the zip code itself depends on the primary key, then city transitively depends on the key through zip code. This violates Third Normal Form (3NF).

<a id="what-is-first-normal-form-1nf"></a>
### Q: What is First Normal Form (1NF)?
**Answer:** A relation is in 1NF if every attribute holds only atomic values, with no repeating groups or multi-valued attributes crammed into a single column, and every row is uniquely identifiable.

<a id="what-is-second-normal-form-2nf"></a>
### Q: What is Second Normal Form (2NF)?
**Answer:** A relation is in 2NF if it's already in 1NF, and every non-key attribute is fully functionally dependent on the entire primary key — relevant specifically for composite primary keys, where a partial dependency would violate it.

<a id="what-is-third-normal-form-3nf"></a>
### Q: What is Third Normal Form (3NF)?
**Answer:** A relation is in 3NF if it's already in 2NF, and it has no transitive dependencies — every non-key attribute depends directly on the primary key, not indirectly through another non-key attribute.

<a id="what-is-boyce-codd-normal-form-bcnf-and-how-does-it-differ-from-3nf"></a>
### Q: What is Boyce-Codd Normal Form (BCNF), and how does it differ from 3NF?
**Answer:** BCNF is a stricter version of 3NF: for every functional dependency A → B, A must be a super key. 3NF has a small exception allowing certain dependencies where B is part of some candidate key even if A isn't a super key — BCNF closes that loophole, making it strictly stronger, since every BCNF relation is in 3NF, but not necessarily vice versa.

<a id="what-is-a-multivalued-dependency-and-what-normal-form-addresses-it"></a>
### Q: What is a multivalued dependency, and what normal form addresses it?
**Answer:** A multivalued dependency exists when one attribute determines a set of values for another attribute, independently of a third attribute — this can cause redundancy even in a relation that's already in BCNF. Fourth Normal Form (4NF) specifically addresses and eliminates this kind of redundancy.

<a id="what-is-denormalization-and-when-might-you-intentionally-use-it"></a>
### Q: What is denormalization, and when might you intentionally use it?
**Answer:** Denormalization deliberately reintroduces some redundancy, often by combining normalized tables or duplicating data, to improve read performance by avoiding expensive joins for very frequently-run queries — a trade-off accepting more complex/careful writes and consistency risk in exchange for faster reads.

<a id="what-are-armstrongs-axioms-and-why-are-they-important-for-functional-dependencies"></a>
### Q: What are Armstrong's Axioms, and why are they important for functional dependencies?
**Answer:** A set of formal inference rules — reflexivity, augmentation, and transitivity — used to derive all the functional dependencies logically implied by a given set of dependencies, forming the theoretical foundation for reasoning about normalization and determining candidate keys systematically rather than by inspection alone.

---

<a id="sql-relational-algebra"></a>
## SQL & Relational Algebra

<a id="what-is-relational-algebra-and-what-is-its-role-in-a-dbms"></a>
### Q: What is relational algebra, and what is its role in a DBMS?
**Answer:** A formal, mathematical query language consisting of operations like selection, projection, union, and join that take one or more relations as input and produce a new relation as output — it's the theoretical foundation a DBMS's query optimizer uses internally to represent and reason about SQL queries, even though users don't write relational algebra directly.

<a id="what-is-the-difference-between-the-selection-and-projection-operations-in-relational-algebra"></a>
### Q: What is the difference between the selection and projection operations in relational algebra?
**Answer:** Selection filters rows from a relation based on a condition, similar to SQL's `WHERE` clause. Projection selects specific columns from a relation, discarding the rest, similar to SQL's column list in a `SELECT` statement.

<a id="what-is-the-difference-between-the-union-intersection-and-set-difference-operations-in-relational-algebra"></a>
### Q: What is the difference between the union, intersection, and set difference operations in relational algebra?
**Answer:** Union combines all tuples from two relations, removing duplicates, requiring both relations to be union-compatible (same structure). Intersection returns only tuples present in both relations. Set difference returns tuples present in the first relation but not the second.

<a id="what-is-a-natural-join-in-relational-algebra-and-how-does-it-relate-to-sqls-join"></a>
### Q: What is a natural join in relational algebra, and how does it relate to SQL's `JOIN`?
**Answer:** A natural join automatically combines two relations based on all attributes they share with the same name, without needing an explicit join condition — it's the relational algebra equivalent of an `INNER JOIN` where the join columns happen to share the same name in both tables.

<a id="what-is-the-cartesian-product-operation-and-how-does-it-relate-to-a-cross-join"></a>
### Q: What is the Cartesian product operation, and how does it relate to a `CROSS JOIN`?
**Answer:** The Cartesian product combines every tuple from one relation with every tuple from another, producing all possible combinations regardless of any relationship between them — directly corresponding to SQL's `CROSS JOIN`.

<a id="what-is-the-difference-between-ddl-dml-dql-dcl-and-tcl-sql-command-categories"></a>
### Q: What is the difference between DDL, DML, DQL, DCL, and TCL SQL command categories?
**Answer:** DDL defines schema structure (`CREATE`, `ALTER`, `DROP`). DML manipulates data (`INSERT`, `UPDATE`, `DELETE`). DQL specifically covers querying data (`SELECT`), sometimes classified under DML instead. DCL controls access permissions (`GRANT`, `REVOKE`). TCL manages transactions (`COMMIT`, `ROLLBACK`, `SAVEPOINT`).

<a id="what-is-a-view-in-relational-database-terms-and-what-relational-algebra-concept-does-it-correspond-to"></a>
### Q: What is a view in relational database terms, and what relational algebra concept does it correspond to?
**Answer:** A view is a saved, named query that behaves like a virtual table. Conceptually, a view is simply a relational algebra expression given a name — querying the view is equivalent to substituting and evaluating that underlying expression against the base tables each time.

<a id="what-is-the-difference-between-tuple-relational-calculus-and-domain-relational-calculus"></a>
### Q: What is the difference between tuple relational calculus and domain relational calculus?
**Answer:** Both are declarative alternatives to relational algebra for expressing queries, describing what you want rather than how to compute it step-by-step. Tuple relational calculus uses variables that range over entire tuples. Domain relational calculus instead uses variables that range over individual domain values, single attribute values, rather than whole tuples.

<a id="how-does-a-query-optimizer-use-relational-algebra-internally-when-processing-a-sql-query"></a>
### Q: How does a query optimizer use relational algebra internally when processing a SQL query?
**Answer:** The optimizer parses the SQL query into an initial relational algebra expression tree, then applies transformation rules, like pushing selections down before joins to filter data as early as possible, to find an equivalent but more efficient expression, before finally choosing a specific physical execution plan to carry it out.

<a id="what-is-the-difference-between-a-scalar-subquery-and-using-a-join-to-achieve-the-same-result"></a>
### Q: What is the difference between a scalar subquery and using a `JOIN` to achieve the same result?
**Answer:** A scalar subquery is nested and returns a single value used within a larger query's expression, and can sometimes be logically executed once per outer row or once total. A `JOIN` combines rows from both tables directly at the same query level, often more efficient since the query optimizer has more flexibility in choosing an execution strategy.

---

<a id="transactions-concurrency-control"></a>
## Transactions & Concurrency Control

<a id="what-is-a-transaction-and-what-are-its-typical-states"></a>
### Q: What is a transaction, and what are its typical states?
**Answer:** A transaction is a sequence of database operations treated as a single logical unit of work. Typical states: active (currently executing), partially committed (finished executing, about to commit), committed (successfully completed and made permanent), failed (an error occurred, can't proceed), and aborted (rolled back after failure).

<a id="what-is-the-difference-between-a-schedule-and-a-serial-schedule"></a>
### Q: What is the difference between a schedule and a serial schedule?
**Answer:** A schedule is any sequence of operations from one or more transactions, however they happen to be interleaved during concurrent execution. A serial schedule is a schedule where transactions execute one completely after another, with no interleaving at all — always correct by definition, but with no concurrency benefit.

<a id="what-is-serializability-and-why-does-it-matter"></a>
### Q: What is serializability, and why does it matter?
**Answer:** A schedule is serializable if its effect on the database is equivalent to some serial execution of the same transactions, even if the actual execution was interleaved for performance. It matters because it guarantees that concurrent execution, despite being interleaved for efficiency, still produces a correct, predictable result as if transactions ran one at a time.

<a id="what-is-the-difference-between-conflict-serializability-and-view-serializability-2"></a>
### Q: What is the difference between conflict serializability and view serializability?
**Answer:** Conflict serializability checks whether a schedule can be transformed into a serial schedule by swapping only adjacent, non-conflicting operations — efficiently checkable via a precedence graph having no cycles. View serializability is a broader condition based on whether transactions read the same values and produce the same final database state as some serial order — every conflict-serializable schedule is view-serializable, but the reverse isn't always true.

<a id="what-is-two-phase-locking-2pl-and-what-are-its-two-phases"></a>
### Q: What is two-phase locking (2PL), and what are its two phases?
**Answer:** A concurrency control protocol with a growing phase, where a transaction can only acquire locks, never release any, and a shrinking phase, where it can only release locks, never acquire more. Once a transaction releases its first lock, it has entered the shrinking phase and can never acquire another lock — this guarantees the resulting schedule is conflict-serializable.

<a id="what-is-the-difference-between-2pl-strict-2pl-and-rigorous-2pl"></a>
### Q: What is the difference between 2PL, strict 2PL, and rigorous 2PL?
**Answer:** Basic 2PL only guarantees serializability, but can still allow cascading rollbacks. Strict 2PL additionally holds all exclusive (write) locks until commit/abort, preventing other transactions from reading uncommitted data. Rigorous 2PL goes further, holding both shared and exclusive locks until commit/abort, simplifying implementation at the cost of slightly reduced concurrency.

<a id="what-is-timestamp-ordering-and-how-does-it-differ-from-lock-based-concurrency-control"></a>
### Q: What is timestamp ordering, and how does it differ from lock-based concurrency control?
**Answer:** Timestamp ordering assigns each transaction a unique timestamp when it starts, and ensures conflicting operations execute in timestamp order — rejecting and typically restarting any operation that would violate this order, rather than making transactions wait for locks. It avoids deadlocks entirely, since no waiting means no circular wait, but can cause more transaction restarts under high contention compared to locking.

<a id="what-is-optimistic-concurrency-control-and-how-does-it-differ-from-pessimistic-approaches"></a>
### Q: What is optimistic concurrency control, and how does it differ from pessimistic approaches?
**Answer:** Optimistic concurrency control lets transactions execute without acquiring locks upfront, instead validating at commit time whether any conflicting changes occurred concurrently — if a conflict is detected, the transaction is aborted and retried. It performs well when actual conflicts are rare, avoiding lock overhead entirely, but can waste work through repeated aborts if contention is actually high.

<a id="what-is-a-cascading-rollback-and-how-do-stricter-locking-protocols-prevent-it"></a>
### Q: What is a cascading rollback, and how do stricter locking protocols prevent it?
**Answer:** A cascading rollback happens when one transaction reads data written by another transaction that later aborts, forcing the first transaction to also abort, potentially triggering a chain reaction of further rollbacks. Strict 2PL prevents this by holding write locks until commit, ensuring no other transaction can ever read data from a transaction that hasn't yet committed.

<a id="what-is-the-difference-between-recoverable-and-non-recoverable-schedules"></a>
### Q: What is the difference between recoverable and non-recoverable schedules?
**Answer:** A recoverable schedule ensures a transaction commits only after any other transaction whose changes it read has already committed — guaranteeing recovery is always possible without needing to undo an already-committed transaction. A non-recoverable schedule violates this, potentially forcing an impossible undo of already-committed work if a dependency later aborts.

<a id="what-is-multi-version-concurrency-control-mvcc-and-what-problem-does-it-solve"></a>
### Q: What is multi-version concurrency control (MVCC), and what problem does it solve?
**Answer:** MVCC maintains multiple versions of a data item, letting readers access an appropriately consistent older snapshot of the data without blocking, or being blocked by, concurrent writers — writers create new versions instead of overwriting in place. This lets reads and writes proceed concurrently without needing to lock against each other, significantly improving read concurrency in databases like PostgreSQL.

<a id="what-is-lock-granularity-and-what-is-multiple-granularity-locking"></a>
### Q: What is lock granularity, and what is multiple granularity locking?
**Answer:** Lock granularity refers to the size of the data item being locked — a whole database, a table, a page, a row, or even a single field. Multiple granularity locking is a protocol using special intention locks on coarser levels, like a table, to efficiently signal that finer-grained locks, like specific rows, are held beneath it, avoiding the need to individually check every fine-grained lock.

---

<a id="indexing-file-organization"></a>
## Indexing & File Organization

<a id="what-is-indexing-in-a-dbms-and-why-is-it-used"></a>
### Q: What is indexing in a DBMS, and why is it used?
**Answer:** An index is an auxiliary data structure that stores a sorted reference to column values and pointers to their corresponding rows/blocks, letting the DBMS quickly locate matching data without scanning the entire file — dramatically speeding up search, range, and sort operations at the cost of some extra storage and slower writes.

<a id="what-is-the-difference-between-a-primary-index-secondary-index-and-clustering-index"></a>
### Q: What is the difference between a primary index, secondary index, and clustering index?
**Answer:** A primary index is built on the primary key of a file that's physically sorted by that same key. A clustering index is built on a non-key field by which the file's records are physically ordered/grouped, even though that field isn't unique. A secondary index is built on any field, providing an additional access path without requiring the underlying file to be physically sorted by that field at all.

<a id="what-is-a-dense-index-vs-a-sparse-index"></a>
### Q: What is a dense index vs. a sparse index?
**Answer:** A dense index has an index entry for every single record in the file. A sparse index has entries for only some records, typically one per disk block, relying on the fact that records within a block can be scanned sequentially once you've located the right block.

<a id="what-is-a-b-tree-and-why-is-it-commonly-used-for-database-indexes"></a>
### Q: What is a B-tree, and why is it commonly used for database indexes?
**Answer:** A self-balancing tree data structure that keeps data sorted and allows searches, sequential access, insertions, and deletions all in logarithmic time. It's especially well-suited for disk-based storage because each node can hold many keys, minimizing the number of disk reads needed to find any given record.

<a id="what-is-the-difference-between-a-b-tree-and-a-b-tree"></a>
### Q: What is the difference between a B-tree and a B+ tree?
**Answer:** In a B-tree, both internal nodes and leaf nodes can store actual data records/pointers. In a B+ tree, all actual data pointers are stored only in the leaf nodes, while internal nodes store just keys used purely for navigation, and leaf nodes are additionally linked together sequentially, making range queries and full sequential scans much more efficient — which is why B+ trees are the standard choice for most database indexes today.

<a id="what-is-hashing-and-how-does-hash-based-indexing-differ-from-b-tree-indexing"></a>
### Q: What is hashing, and how does hash-based indexing differ from B-tree indexing?
**Answer:** Hashing applies a hash function to a key to compute the exact location where a record should be stored/found, giving very fast average-case lookups for exact-match queries. Unlike a B-tree, hash indexes don't preserve any ordering, so they're not useful for range queries or sorted retrieval — B-tree indexes remain necessary whenever ordering matters.

<a id="what-is-the-difference-between-static-hashing-and-dynamic-hashing"></a>
### Q: What is the difference between static hashing and dynamic hashing?
**Answer:** Static hashing uses a fixed number of buckets determined upfront — if data grows significantly beyond what was planned for, buckets become overloaded and performance degrades, requiring a full, expensive reorganization. Dynamic hashing can grow the number of buckets incrementally as data grows, avoiding that costly full reorganization.

<a id="what-is-file-organization-and-what-are-the-common-types"></a>
### Q: What is file organization, and what are the common types?
**Answer:** File organization describes how records are physically arranged on disk. Common types: heap/pile organization (records stored in no particular order, simple insertion but slow search), sequential organization (records physically sorted by a key field, efficient for range scans but slower insertion), and hashed organization (records placed by a hash function, fast exact-match lookup).

<a id="what-is-a-composite-index-and-how-does-column-order-affect-its-usefulness"></a>
### Q: What is a composite index, and how does column order affect its usefulness?
**Answer:** An index built on multiple columns together. Order matters significantly — an index on columns (a, b) can efficiently support queries filtering on `a` alone, or `a` and `b` together, following a left-to-right prefix rule, but generally can't efficiently support a query filtering only on `b` without `a`.

<a id="what-is-the-trade-off-between-having-more-indexes-on-a-table"></a>
### Q: What is the trade-off between having more indexes on a table?
**Answer:** More indexes speed up read queries that can use them, but slow down write operations, since every index must also be updated whenever the underlying data changes, and each index consumes additional disk space.

---

<a id="deadlocks-recovery"></a>
## Deadlocks & Recovery

<a id="what-are-the-four-necessary-conditions-for-a-deadlock"></a>
### Q: What are the four necessary conditions for a deadlock?
**Answer:** Mutual exclusion (a resource can be held by only one transaction at a time), hold and wait (a transaction holds one resource while waiting for another), no preemption (a resource can't be forcibly taken from a transaction holding it), and circular wait (a cycle of transactions, each waiting for a resource held by the next in the cycle).

<a id="what-is-the-difference-between-deadlock-prevention-avoidance-and-detection"></a>
### Q: What is the difference between deadlock prevention, avoidance, and detection?
**Answer:** Prevention eliminates one of the necessary conditions upfront, guaranteeing deadlocks structurally can't occur, but often limiting concurrency significantly. Avoidance dynamically checks before granting each lock request whether doing so could ever lead to a deadlock, denying the request if so. Detection allows deadlocks to potentially occur, but periodically checks for them and resolves any found by aborting a victim transaction.

<a id="what-is-a-wait-for-graph-and-how-is-it-used-to-detect-deadlocks"></a>
### Q: What is a wait-for graph, and how is it used to detect deadlocks?
**Answer:** A graph where each transaction is a node, and an edge from transaction A to transaction B means A is waiting for a resource held by B. A deadlock exists if and only if this graph contains a cycle — the DBMS periodically checks for cycles and, if found, aborts one of the transactions in the cycle to break it.

<a id="what-is-the-difference-between-the-wait-die-and-wound-wait-deadlock-prevention-schemes"></a>
### Q: What is the difference between the wait-die and wound-wait deadlock prevention schemes?
**Answer:** Both use transaction timestamps to decide what happens when a transaction requests a resource held by another. In wait-die, an older transaction waits for a younger one, but a younger transaction requesting from an older one is forced to abort and restart. In wound-wait, an older transaction forces a younger one holding the resource to abort and take the resource, while a younger transaction requesting from an older one simply waits.

<a id="what-is-a-checkpoint-and-why-is-it-used-in-database-recovery"></a>
### Q: What is a checkpoint, and why is it used in database recovery?
**Answer:** A checkpoint periodically records the current, consistent state of the database to stable storage, along with a note of which transactions were active at that moment. After a crash, recovery only needs to examine the log from the most recent checkpoint forward, rather than replaying the entire transaction log from the very beginning, significantly speeding up recovery time.

<a id="what-is-the-difference-between-the-redo-and-undo-phases-of-database-recovery"></a>
### Q: What is the difference between the redo and undo phases of database recovery?
**Answer:** The redo phase reapplies the effects of transactions that had already committed but whose changes might not have been fully written to disk yet before the crash, ensuring durability. The undo phase reverses the effects of transactions that were still in progress at the time of the crash, ensuring atomicity by discarding their partial work.

<a id="what-is-shadow-paging-and-how-does-it-differ-from-log-based-recovery"></a>
### Q: What is shadow paging, and how does it differ from log-based recovery?
**Answer:** Shadow paging maintains two complete page tables — a current one being actively modified, and a shadow one representing the last consistent, committed state — committing a transaction simply means atomically switching the shadow table to point to the current one. Unlike log-based recovery, it doesn't need a separate log or undo/redo operations, but it can suffer from data fragmentation over time and complicates supporting concurrent transactions.

<a id="what-is-the-write-ahead-logging-wal-rule-and-why-is-it-fundamental-to-crash-recovery"></a>
### Q: What is the write-ahead logging (WAL) rule, and why is it fundamental to crash recovery?
**Answer:** The rule that log records describing a change must be written to stable storage before the actual data change itself is written to disk. This guarantees that if a crash happens mid-write, the log always has enough information to correctly redo or undo the incomplete operation.

---

<a id="distributed-databases-nosql"></a>
## Distributed Databases & NoSQL

<a id="what-is-a-distributed-database-and-what-are-its-main-advantages"></a>
### Q: What is a distributed database, and what are its main advantages?
**Answer:** A database where data is stored across multiple physical locations/servers, potentially geographically dispersed, while appearing to users as a single logical database. Advantages: improved reliability/availability, better performance for geographically distributed users, and the ability to scale beyond what a single server can handle.

<a id="what-is-data-fragmentation-in-a-distributed-database-and-what-are-its-types"></a>
### Q: What is data fragmentation in a distributed database, and what are its types?
**Answer:** Splitting a database's data across multiple sites. Horizontal fragmentation splits a table's rows across sites. Vertical fragmentation splits a table's columns across sites. Mixed fragmentation combines both approaches.

<a id="what-is-the-cap-theorem-and-what-does-it-state"></a>
### Q: What is the CAP theorem, and what does it state?
**Answer:** The CAP theorem states that a distributed system can only guarantee at most two of the following three properties simultaneously during a network partition: Consistency (every read receives the most recent write), Availability (every request receives a non-error response), and Partition tolerance (the system continues operating despite network failures splitting it). Since partition tolerance is essentially mandatory for any real distributed system, the practical trade-off is really between consistency and availability during an actual partition.

<a id="what-is-eventual-consistency-and-where-is-it-commonly-used"></a>
### Q: What is eventual consistency, and where is it commonly used?
**Answer:** A consistency model where, if no new updates are made to a piece of data, all replicas will eventually converge to the same value — but at any given moment, different replicas might temporarily return different, stale values. Common in NoSQL databases and distributed systems favoring availability/performance over strict, immediate consistency.

<a id="what-is-the-difference-between-a-distributed-database-and-a-nosql-database"></a>
### Q: What is the difference between a distributed database and a NoSQL database?
**Answer:** These are somewhat orthogonal concepts. Distributed describes where and how data is physically stored across multiple nodes, while NoSQL describes the data model (document, key-value, column-family, graph) as opposed to the traditional relational model. Many NoSQL databases happen to be distributed by design, but a database can be distributed while still being relational, or NoSQL while running on a single node.

<a id="what-are-the-main-categories-of-nosql-databases"></a>
### Q: What are the main categories of NoSQL databases?
**Answer:** Key-value stores (simple key-to-value lookups, like Redis), document stores (flexible, semi-structured documents, like MongoDB), column-family stores (wide, sparse columns grouped by row key, like Cassandra), and graph databases (nodes and relationships as first-class citizens, like Neo4j) — each optimized for different access patterns.

<a id="what-is-a-two-phase-commit-protocol-and-what-problem-does-it-solve-in-distributed-transactions"></a>
### Q: What is a two-phase commit protocol, and what problem does it solve in distributed transactions?
**Answer:** A protocol ensuring all participating nodes in a distributed transaction either all commit or all abort together, even across multiple separate databases/servers. In the first (prepare) phase, a coordinator asks all participants if they're ready to commit; only if all respond yes does the coordinator send a second (commit) phase message telling everyone to actually commit — otherwise it tells everyone to abort.

<a id="what-is-data-replication-in-a-distributed-database-and-what-are-its-trade-offs"></a>
### Q: What is data replication in a distributed database, and what are its trade-offs?
**Answer:** Storing multiple copies of the same data across different nodes, improving availability and read performance. The trade-off is the added complexity and overhead of keeping all replicas synchronized/consistent, especially under concurrent writes.

---

<a id="database-security"></a>
## Database Security

<a id="what-is-database-security-and-why-is-it-important"></a>
### Q: What is database security, and why is it important?
**Answer:** The set of measures protecting a database from unauthorized access, misuse, or corruption — important because databases often store an organization's most sensitive and valuable data, making them a prime target for attacks.

<a id="what-is-the-difference-between-authentication-and-authorization-in-database-security"></a>
### Q: What is the difference between authentication and authorization in database security?
**Answer:** Authentication verifies who a user is, typically via credentials like a username/password. Authorization determines what that authenticated user is actually allowed to do — which specific data and operations they can access — typically governed by assigned roles or permissions.

<a id="what-is-sql-injection-and-how-do-you-prevent-it"></a>
### Q: What is SQL injection, and how do you prevent it?
**Answer:** An attack where malicious SQL code is inserted into an application's input fields and gets executed by the database because user input was concatenated directly into a query string instead of being properly separated from the query's actual logic. Prevent it by always using parameterized queries rather than string concatenation, and by validating/sanitizing user input as an additional defense layer.

<a id="what-is-role-based-access-control-rbac-and-why-is-it-useful-for-managing-database-permissions"></a>
### Q: What is Role-Based Access Control (RBAC), and why is it useful for managing database permissions?
**Answer:** A security model where permissions are granted to defined roles rather than directly to individual users, and users are then assigned one or more roles — greatly simplifying permission management across many users who share similar access needs.

<a id="what-is-the-principle-of-least-privilege-and-how-does-it-apply-to-database-access"></a>
### Q: What is the principle of least privilege, and how does it apply to database access?
**Answer:** Granting each user or application account only the minimum permissions actually necessary for their specific function — limiting the potential damage if that particular credential is ever compromised.

<a id="what-is-encryption-at-rest-vs-encryption-in-transit"></a>
### Q: What is encryption at rest vs. encryption in transit?
**Answer:** Encryption at rest protects data stored on disk, so it remains unreadable even if the physical storage media itself is stolen or improperly accessed. Encryption in transit, typically via TLS/SSL, protects data as it travels over the network between the client and the database server.

<a id="what-is-database-auditing-and-why-is-it-used"></a>
### Q: What is database auditing, and why is it used?
**Answer:** Recording a log of who accessed or modified what data, and when — used for detecting suspicious activity, satisfying regulatory/compliance requirements, and providing an investigative trail after a security incident.

<a id="what-is-data-masking-and-when-would-you-use-it"></a>
### Q: What is data masking, and when would you use it?
**Answer:** A technique that obscures or replaces sensitive real data with realistic but fake substitute values, typically used when giving developers, testers, or analysts access to a copy of production-like data without exposing actual sensitive customer information they don't genuinely need to see.

---

<a id="common-conceptual-coding-challenges"></a>
## Common Conceptual & Coding Challenges

<a id="given-a-relation-with-a-composite-primary-key-how-would-you-identify-whether-its-in-2nf"></a>
### Q: Given a relation with a composite primary key, how would you identify whether it's in 2NF?
**Answer:** Check whether every non-key attribute depends on the entire composite key. It would be violated if some non-key attribute depended on just part of that key — e.g. in an order-line relation keyed on (OrderID, ProductID), a `ProductName` attribute likely depends only on `ProductID` alone, a partial dependency violating 2NF; `ProductName` should be moved to its own Products table.

<a id="given-a-functional-dependency-set-how-would-you-determine-the-candidate-keys-of-a-relation"></a>
### Q: Given a functional dependency set, how would you determine the candidate key(s) of a relation?
**Answer:** Compute the "closure" of different attribute combinations under the given functional dependencies, repeatedly applying the dependencies to see what additional attributes can be derived. An attribute set is a candidate key if its closure includes all attributes of the relation, and no proper subset of it also has that property.

<a id="how-would-you-design-a-schema-in-3nf-for-a-simple-library-management-system"></a>
### Q: How would you design a schema, in 3NF, for a simple library management system?
**Answer:** Separate tables for Books (book ID, title, author), Members (member ID, name, contact info), and a BorrowRecords junction table (borrow ID, book ID, member ID, borrow date, return date) linking books to members via foreign keys — avoiding storing member details redundantly on every borrow record.

<a id="given-a-precedence-graph-for-a-schedule-how-would-you-determine-if-its-conflict-serializable"></a>
### Q: Given a precedence graph for a schedule, how would you determine if it's conflict-serializable?
**Answer:** Build the graph with a node per transaction, and a directed edge whenever one transaction has an operation that conflicts with, and comes before, a later operation of another transaction on the same data item. The schedule is conflict-serializable if and only if this graph is acyclic — a topological sort of the graph then gives a valid equivalent serial order.

<a id="given-a-set-of-transactions-and-lock-requests-how-would-you-identify-whether-a-deadlock-occurs"></a>
### Q: Given a set of transactions and lock requests, how would you identify whether a deadlock occurs?
**Answer:** Build a wait-for graph from the lock requests and grants, with an edge from one transaction to another if the first is waiting on a lock held by the second. A deadlock exists if and only if the graph contains a cycle, and the transactions involved in that cycle are deadlocked.

<a id="how-would-you-compute-the-number-of-block-accesses-needed-for-a-linear-search-vs-a-binary-search-on-a-sorted-indexed-file"></a>
### Q: How would you compute the number of block accesses needed for a linear search vs. a binary search on a sorted, indexed file?
**Answer:** A linear search on a file with `n` blocks requires up to `n` block accesses in the worst case. A binary search on the same sorted file requires roughly log base 2 of `n` block accesses — a dramatic improvement, which is exactly why indexing matters so much for large tables.

<a id="given-a-relation-how-would-you-write-the-relational-algebra-expression-to-find-rows-matching-a-condition-and-only-certain-columns"></a>
### Q: Given a relation, how would you write the relational algebra expression to find rows matching a condition and only certain columns?
**Answer:** Combine selection and projection: project the desired columns from the selection of rows matching the condition on the relation — selection first filters rows, and projection then narrows down to just the desired columns from that filtered result.

<a id="given-two-relations-how-would-you-write-the-relational-algebra-expression-for-a-natural-join"></a>
### Q: Given two relations, how would you write the relational algebra expression for a natural join?
**Answer:** The natural join operator automatically matches and combines rows based on all attributes with the same name shared between the two relations, without needing an explicit join condition specified.

<a id="how-would-you-determine-whether-a-given-database-design-suffers-from-an-update-anomaly"></a>
### Q: How would you determine whether a given database design suffers from an update anomaly?
**Answer:** An update anomaly exists if a single real-world fact is stored redundantly across multiple rows, requiring every copy to be updated consistently, risking some being missed. Fix it by normalizing — moving the redundant fact into its own dedicated table, referenced by a foreign key, so it only needs to be stored and updated in exactly one place.

<a id="given-a-scenario-with-concurrent-transactions-what-happens-if-you-apply-strict-two-phase-locking"></a>
### Q: Given a scenario with concurrent transactions, what happens if you apply strict two-phase locking?
**Answer:** Each transaction acquires all needed locks during its growing phase, holds all write locks until it actually commits or aborts, and only releases everything at that point. The resulting schedule is guaranteed to be conflict-serializable and free of cascading rollbacks, since no other transaction could have read data written by a transaction that hadn't yet committed.

---

<a id="behavioral-scenario-based-questions"></a>
## Behavioral / Scenario-Based Questions

<a id="how-would-you-approach-designing-a-database-schema-for-a-new-application-from-scratch"></a>
### Q: How would you approach designing a database schema for a new application from scratch?
**Answer:** Start by identifying the core entities and their relationships, often sketching an ER diagram first, normalize the design to at least 3NF to avoid redundancy and anomalies, define appropriate keys and constraints to enforce data integrity, and only consider selective denormalization later, once real query patterns and performance bottlenecks are actually understood.

<a id="how-would-you-diagnose-and-resolve-a-deadlock-occurring-in-a-production-system"></a>
### Q: How would you diagnose and resolve a deadlock occurring in a production system?
**Answer:** Rely on the database's automatic deadlock detection to roll back one of the involved transactions, but investigate the actual application code causing it, commonly two transactions acquiring the same set of locks in a different order, and fix it going forward by enforcing a consistent lock-acquisition order across the codebase, or reducing transaction scope/duration.

<a id="how-would-you-decide-between-normalizing-fully-and-selectively-denormalizing-part-of-a-schema"></a>
### Q: How would you decide between normalizing fully and selectively denormalizing part of a schema?
**Answer:** Weigh the actual read/write ratio and query patterns for that specific data — normalize by default for data integrity and to avoid update anomalies, but consider denormalizing a specific, well-understood, frequently-queried hot path where join/aggregation performance genuinely can't keep up otherwise.

<a id="how-would-you-explain-the-trade-off-between-strong-consistency-and-high-availability-to-a-non-technical-stakeholder"></a>
### Q: How would you explain the trade-off between strong consistency and high availability to a non-technical stakeholder?
**Answer:** Frame it around a concrete scenario — during a network problem, the system can either wait to make sure everyone sees the exact same, most up-to-date information before responding, or respond immediately with whatever information it currently has, even if it might be slightly out of date for some users — and the CAP theorem says you fundamentally can't have perfectly both at the same time during that kind of failure.

<a id="how-would-you-approach-recovering-a-database-after-a-server-crash"></a>
### Q: How would you approach recovering a database after a server crash?
**Answer:** Rely on the write-ahead log combined with the most recent checkpoint — redo the effects of transactions that had committed but weren't fully flushed to disk before the crash, and undo the effects of transactions that were still in progress and uncommitted at the time of the crash.

<a id="how-would-you-choose-between-a-relational-database-and-a-nosql-database-for-a-new-project"></a>
### Q: How would you choose between a relational database and a NoSQL database for a new project?
**Answer:** Consider whether the data has a stable, well-defined relational structure with a need for strong consistency and complex multi-table queries, versus rapidly evolving/flexible schemas, very high write throughput, or natural horizontal scaling needs — and don't assume it's an all-or-nothing choice, since many real systems use both for different parts of the application.

<a id="how-would-you-investigate-a-query-thats-performing-much-slower-than-expected-in-production"></a>
### Q: How would you investigate a query that's performing much slower than expected in production?
**Answer:** Examine the query's execution plan to see whether it's using appropriate indexes or falling back to a full table scan, check whether statistics are up to date, look at the actual data volume involved versus what the query was originally designed/tested against, and check for lock contention if concurrent transactions might be blocking each other.

<a id="how-would-you-approach-reviewing-a-teammates-proposed-database-schema-in-a-design-review"></a>
### Q: How would you approach reviewing a teammate's proposed database schema in a design review?
**Answer:** Check that the design is appropriately normalized, or that any denormalization is a deliberate, justified choice, verify primary/foreign keys and constraints are correctly defined, look for any obviously missing indexes on columns that will clearly be filtered/joined on frequently, and confirm the schema realistically accommodates how the data is expected to grow and change over time.

---

<a id="how-to-use-this-guide"></a>
## How to Use This Guide

- **A few days before an interview or exam?** Go section by section, top to bottom — each one builds on the last, from basics to distributed systems and security.
- **Revising the night before?** Jump straight to 🔥 Most Asked / Tricky Questions, then skim section headers for anything you're unsure about.
- **During quick revision:** Use `Ctrl+F` (or `Cmd+F`) to jump straight to a keyword or topic instead of scrolling.
- **After every interview:** Come back and add any question you got asked that isn't already here — this file is meant to grow with you.

Good luck — you've got this. 🚀
