---
layout: post
title: Unit 1- Introduction to Database Systems
date: "2025-02-21"
description: You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. # Add post description (optional)
img: dbms.png # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [DBS101]
---

## My Initial Understanding of Databases

Before learning about database systems, I had a basic idea of what a database was. I thought of it as an organized way to store and find information easily. I knew that databases were useful, but I didn’t know much about how they developed over time, the different ways data could be structured, or how databases actually work behind the scenes.

## How My Perspective Has Changed

My understanding of databases has grown so much. I’ve realized that they’re more than just collections of tables—they have structured designs, multiple levels of abstraction, and different models suited for various applications. Here are some of my key takeaways:

## 1.1 View of Data

I used to think databases were just structured collections of data, but I’ve now learned that data can be organized and represented in different ways. Some of the main models include:

* Entity-Relationship (E-R) Model – Helps visualize relationships between entities, making conceptual design easier.
* Relational Model – Organizes data into tables (rows and columns) with well-defined relationships.
* Semi-structured Data Models – Used when data doesn’t fit neatly into tables, like XML, JSON, or NoSQL databases.
* Object-Based Model – Follows object-oriented principles, where data is stored as objects with attributes and behaviors.

![dbs-hw](/assets/img/dbs-hw.jpeg)

## 1.2 The Purpose and Importance of Database Systems

At first, I thought databases were just for storing data, but I now understand that they play a crucial role in efficiently managing and processing information. They help solve major challenges of traditional file-based systems, such as:

* Data redundancy and inconsistency – Databases provide a single, accurate source of truth.
* Difficulty in accessing data – Query languages (like SQL) allow structured and flexible retrieval.
* Data isolation and integrity issues – Constraints and relationships ensure data consistency.
* Security challenges – Authentication and authorization help protect sensitive data.

## 1.3 History of Database Systems

Learning about the evolution of databases gave me a new appreciation for how far data management has come:

* File-Based Systems – Early storage methods were basic and lacked structure.
* Hierarchical and Network Models – Introduced more structure but had rigid relationships.
* Relational Model (1970s - Edgar F. Codd) – Revolutionized databases by structuring data into tables with relationships.
* Object-Oriented & NoSQL Databases – Designed for modern applications, handling large, unstructured datasets.

## 1.4 Database-System Applications

Databases are everywhere! Some key areas where they’re used include:

* Banking – Storing transaction records and account details.
* E-commerce – Managing customer data, inventory, and transactions.
* Healthcare – Keeping patient records and medical histories.
* Social Media – Handling massive amounts of user-generated content like posts, images, and videos.
* Cloud Computing – Providing scalable, distributed database solutions.

## 1.5 Database Languages

I didn’t realize there were different types of database languages, each serving a specific purpose:

* Data Definition Language (DDL) – Used to set up and modify the structure of a database (e.g., CREATE, ALTER, DROP).
* Data Manipulation Language (DML) – Handles retrieving and updating data (e.g., SELECT, INSERT, UPDATE, DELETE).

## 1.6 Database Design

I learned that database design is crucial for efficient data storage and retrieval. Important aspects include:

* Conceptual Design – Using the E-R Model to define relationships between data.
* Logical Design – Converting conceptual designs into structured relational schemas.

## 1.7 Database Engine

Key components of a database engine include:

* Storage Management – Organizes data efficiently.

* Query Processing – Optimizes query execution.

* Transaction Management – Ensures reliability through ACID properties (Atomicity, Consistency, Isolation, Durability).

## 1.8 Database and Application Architecture

Databases interact with applications in different ways:

![3-tier architecture](/assets/img/3-tier-architecture.jpeg)

* Single-tier Architecture – Database and application run on the same system.
* Two-tier Architecture – A client communicates directly with a database server.
* Three-tier Architecture – An additional middle layer (API or web server) improves scalability.
* Distributed Databases – Data is spread across multiple locations for better reliability and speed.

## Homework

![dbs-dbms](/assets/img/dbs-dbms.jpeg)

## Conclusion

This unit has helped me understand databases much better. I now see that they do more than store data—they help organize and manage information efficiently. Learning about data models, architecture, and languages has been really helpful. I’m excited to learn more and see how databases are used in real-life situations.

