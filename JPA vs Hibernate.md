# ORM (Object-Relational Mapping)
<p>Is the method of querying and manipulating data from a database using an object-oriented paradigm/programming language.By using this method, we are able to interact with a relational database without having to use SQL.

- Java Persistence API (JPA)
 Is a Java specification that deals with persistent data in Java applications. JPA is primarily concerned with the ORM layer.

- One of the most widely used Java ORM frameworks is Hibernate.

 In short, the main difference between Hibernate and JPA is that Hibernate is a framework whereas JPA is an API specification focused mainly on ORM.

## What is JPA?
<p> It stands for Java Persistence API, a Java specification that provides an object mapping facility to relational databases for Java applications. It provides a mechanism for managing persistence and object-relational mapping. JPA defines these mappings internally rather than depending on vendor-specific implementations.

<p>JPA represents how to define POJO (Plain Old Java Object) as an entity and manage it with relations using some meta configurations. They are defined either by annotations or by XML files.

<p>It is a Java specification that gives some functionality and standard to ORM tools.
<p>It is considered as a link between an object-oriented model and a relational database system.
<p>JPA does not conduct any functioning by itself. Therefore, it needs implementation. Hence, for data persistence ORM tools like Hibernate implements JPA specifications.




## What is Hibernate?
<p>Hibernate is an open-source, lightweight ORM tool that provides Object-Relational persistence and query service for any Java application.
It is one of the most popular implementations of Java Persistence API.
It helps to map java objects to the database and helps to reduce common persistence-related programming tasks. This task can be done quickly using XML files, and you do not need to write any line of code.
Hibernate ORM framework is designed by Red Hat.It supports a cross-platform JVM and is written in Java.

 The main feature of Hibernate is to map the Java classes to database tables. 
 - Hibernate is an implementation of JPA guidelines.
- It helps in mapping Java data types to SQL data types.
- It is the contributor of JPA.



## Difference Between JPA and Hibernate


| JPA | Hibernate |
|--------------- |---------------|
|JPA is responsible for managing relational databases in Java applications|Hibernate is an ORM tool used for saving the state of the Java object in the database|
|javax.persistence package |org.hibernate package|
|JPA is the Java specification and not the implementation|Hibernate is an implementation of JPA|
|It uses Java Persistence Query Language (JPQL) is an object-oriented query language to perform database operations|It uses Hibernate Query Language (HQL) is an object-oriented query language to perform database operations|
|It uses the EntityManager interface to create, read, and delete operations for instances of mapped entity classes|It uses a Session interface to create, read, and delete operations for instances of mapped entity classes|
|It  uses the EntityManagerFactory interface to interact with the entity manager factory|It uses the SessionFactory interface for creating Session instances.|


