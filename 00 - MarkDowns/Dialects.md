> Dialect : the word dialect means mothertongue, or native/local language. here it means the mothertongue or local language or our database. PostgreSQL has its own mothertongue, mySQL has its own mothertongue


**spring.jpa.database-platform**: This property specifies the Hibernate dialect to use. A dialect in Hibernate is a class that provides specific details about the SQL dialect for a particular database. It helps Hibernate generate SQL that is optimized for the database you're using.  

**org.hibernate.dialect.PostgreSQLDialect**: This is the fully qualified class name of the dialect implementation for PostgreSQL. It tells Hibernate that your application is using PostgreSQL as the database, so Hibernate should generate SQL queries and statements that are compatible with PostgreSQL.

> basically specifying Dialect is process which gives backend a manual about our database like SQL queries, specific features(datatype, functions, keywords)

```bash
# PostgreSQL Dialect
spring.jpa.database-platform=org.hibernate.dialect.PostgreSQLDialect
```
```bash
# mySQL Dialect
spring.jpa.database-platform=org.hibernate.dialect.MySQLDialect
```
```bash
# OracleDB Dialect
spring.jpa.database-platform=org.hibernate.dialect.OracleDialect
```