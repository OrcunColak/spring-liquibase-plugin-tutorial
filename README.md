# Read Me First

The original idea is from  
https://leonardopache.medium.com/db-changes-management-with-liquibase-3f7b2d7dfd6e

This project does not autoconfigure liquibase. We need to run the plugin manually

To populate the database run

```
mvn liquibase:update
```

To see history run

```
mvn liquibase:history
```
