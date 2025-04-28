---
layout: post
title: Unit 5 - Relational Database Design
date: "2025-04-28"
description: Essential principles of relational database design, normalization, decomposition, and temporal data modeling.
img: rd.png # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [DBS101]
---

## My Initial Understanding of Relational Database Design

Before starting this unit, I thought relational database design was mostly about organizing tables neatly and ensuring data could be retrieved easily. I was familiar with basic concepts like tables, primary keys, and foreign keys, but I hadn’t realized how deep and formalized the process of good relational design truly is. I had little understanding of functional dependencies, decomposition principles, or the subtle trade-offs involved in advanced normalization.

## How My Perspective Has Changed

This unit transformed my understanding of database design from a simple, common-sense task into a precise science. I now see relational database design as a careful balancing act—ensuring minimal redundancy, preserving data integrity, and maintaining efficiency. Concepts like multivalued dependencies, temporal data modeling, and advanced normal forms opened my eyes to the complexity and power behind professional database systems.

## 5.1 Features of Good Relational Designs

I learned that a good relational design ensures each entity is represented by its own relation, minimizes null values, prevents spurious tuples during joins, and eliminates redundancy and anomalies. A clean design not only saves storage but also avoids hidden pitfalls like update, insertion, and deletion anomalies that can quietly corrupt data over time.

## 5.2 Decomposition Using Functional Dependencies

Decomposition is about breaking down larger tables into smaller, better-structured ones without losing information. The concept of **lossless decomposition** is crucial here—it ensures that when we join decomposed tables back, we get exactly the original table without unwanted (spurious) rows. Functional dependencies guide us on how to perform this decomposition safely and meaningfully.

## 5.3 Normal Forms

Normalization organizes data into progressively stricter normal forms:
- **1NF** eliminates multi-valued and composite attributes.
- **2NF** removes partial dependencies on a part of a primary key.
- **3NF** removes transitive dependencies, ensuring that non-prime attributes depend only on the keys.
- **BCNF** tightens the rules further, requiring every determinant to be a superkey.
- Higher forms like **4NF** and **5NF** deal with more complex constraints like multivalued and join dependencies.
Normalization is not just an academic exercise—it directly prevents data corruption, reduces redundancy, and simplifies future queries and updates.

![nf](/assets/img/nf.png)


## 5.4 Functional-Dependency Theory

Functional dependencies (FDs) are the backbone of relational database theory. I discovered how to compute the **closure** of a set of FDs, use **Armstrong’s axioms** (reflexivity, augmentation, transitivity), and reason about how attributes depend on each other. Understanding **canonical covers** helped me simplify sets of FDs without losing their meaning, a powerful tool when optimizing schemas.

## 5.5 Algorithms for Decomposition Using Functional Dependencies

There are systematic algorithms for decomposing relations:
- **BCNF decomposition** ensures strong normalization but may sacrifice dependency preservation.
- **3NF decomposition** (synthesis approach) guarantees dependency preservation while still reducing redundancy.
Learning these algorithms showed me that decomposition is not random—it follows clear, logical steps to balance normalization and practicality.

## 5.6 Decomposition Using Multivalued Dependencies

Sometimes even BCNF isn’t enough. **Multivalued dependencies** occur when one attribute can vary independently of another, like a professor having multiple addresses and multiple departments. Decomposing based on multivalued dependencies into **Fourth Normal Form (4NF)** removes these hidden redundancies, ensuring that tuples are clean and independent.

![mvd](/assets/img/mvd.png)

## 5.7 More Normal Forms

Beyond 4NF, there are even stricter forms:
- **Fifth Normal Form (5NF)** deals with **join dependencies**, ensuring that every valid combination of data can be reconstructed from smaller relations.
- **Domain-Key Normal Form (DKNF)** is the ultimate goal, where all constraints are a result of domain definitions or keys.
However, practical databases rarely go beyond 3NF or BCNF, as the complexity often outweighs the benefits for real-world systems.

## 5.8 Atomic Domains and First Normal Form

1NF emphasizes that every attribute must have atomic (indivisible) values. I learned why composite or multi-valued attributes—although sometimes tempting—cause trouble in the long run. By ensuring atomic domains, databases become simpler to query, update, and reason about.

## 5.9 Database-Design Process

A well-designed database often starts with a carefully crafted **Entity-Relationship (E-R) diagram**, but normalization is the critical second step to fix any oversights. I also learned that real-world projects sometimes intentionally **denormalize** parts of the database to optimize performance, accepting some redundancy in exchange for faster queries.

## 5.10 Modelling Temporal Data

Adding **time** to a database introduces a new layer of complexity. Functional dependencies that hold at one moment may not hold across time. I learned how to model temporal data by adding valid time periods and ensuring primary keys prevent overlapping records. Temporal modeling ensures databases can faithfully record changing realities without losing historical information.

![tdata](/assets/img/tdata.png)

## Key Takeaways from the Unit

* Good relational design minimizes redundancy, nulls, and anomalies.
* Functional dependencies and canonical covers are essential tools for schema optimization.
* Normalization is a structured, multi-level process balancing data integrity and practical needs.
* Multivalued dependencies and temporal data add complexity, but they can be handled with careful design.
* Database design is an iterative, thoughtful process requiring both theory and pragmatism.

## What I Learned and Why It Matters

Understanding relational database design at this level has made me realize that databases are far more than just tables and columns—they are intricate systems that must be carefully architected. Good design prevents countless future problems, improves scalability, maintains data integrity, and ensures reliable query performance. These skills are foundational for any role in backend development, data engineering, or system architecture.

## Personal Growth and Reflection

This unit has changed the way I think about databases forever. I now appreciate the precision, foresight, and discipline needed to create databases that are efficient, reliable, and adaptable. I feel much more confident about designing schemas from scratch and reasoning about their correctness and efficiency. Most importantly, I have learned to balance theory and practice—knowing when to normalize rigorously, and when to adapt for real-world needs.

## Conclusion

Relational database design is both an art and a science. This unit provided me with the theoretical foundation and practical tools needed to build databases that are not just functional, but truly robust and future-proof. From understanding functional dependencies to modeling temporal data, I now have a deep appreciation for the complexity and elegance of relational systems. I am excited to apply these skills in real-world projects and continue refining them as I grow in my career.

