# @SequenceGenerator OR @TableGenerator
- It is the name of the primary key generator as specified in the **@SequenceGenerator** or **@TableGenerator** annotation.
- These two annotations controls how database sequence or table is mapped.
- Can be used on the entity class or on the primary key field or property.
# @GeneratedValue
- used in conjunction with @Id annotation to automatically generate unique values for primary key columns within our database tables.
#### The @GeneratedValue annotation provides us with different strategies for the generation of primary keys which are as follows : 
1. GenerationType.IDENTITY: generate the primary key value by the database itself using the auto-increment column option.
2. GenerationType.AUTO: default strategy and the persistence provider which automatically selects an appropriate generation strategy based on the database usage.
3. GenerationType.TABLE: uses a separate database table to generate primary key values.The persistence provider manages this table and uses it to allocate unique values for primary keys.
4. GenerationType.SEQUENCE: uses a database sequence to generate primary key values.It requires the usage of database sequence objects.