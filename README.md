# Read Me First

The original idea is from  
https://leonardopache.medium.com/db-changes-management-with-liquibase-3f7b2d7dfd6e

This project does not have any source code so it does not autoconfigure liquibase. We need to run the plugin manually

To create first changelog run

```
mvn liquibase:generateChangeLog -Dliquibase.outputChangeLogFile=my-changelog.xml
```

To populate the database run

```
# Creates databasechangelog and databasechangeloglock tables
mvn compile

# Creates my tables
mvn liquibase:update
```

To see history run

```
mvn liquibase:history
```
