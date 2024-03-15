# Relational Data Access

Relational Data Access is a Spring Boot Project designed to help you get to grips with the Spring Boot Framework.

## Installation

* [Fork the repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo)

* Clone your own repo on your local machine

* Add the upstream pointing to the original repo (the one who has been fork) 

## Usage

* Build the project

```bash
   mvn dependency:resolve
```

* Launch the application

```bash
    mvn spring-boot:run
```

* Result expected

```bash
[...]
2024-03-15T11:49:26.277+01:00  INFO 21708 --- [relational-data-access] [           main] com.zaxxer.hikari.HikariDataSource       : HikariPool-1 - Start completed.
2024-03-15T11:49:26.291+01:00  INFO 21708 --- [relational-data-access] [           main] c.e.f.r.RelationalDataAccessApplication  : Inserting customer record for John Woo
2024-03-15T11:49:26.292+01:00  INFO 21708 --- [relational-data-access] [           main] c.e.f.r.RelationalDataAccessApplication  : Inserting customer record for Jeff Dean
2024-03-15T11:49:26.292+01:00  INFO 21708 --- [relational-data-access] [           main] c.e.f.r.RelationalDataAccessApplication  : Inserting customer record for Josh Bloch
2024-03-15T11:49:26.292+01:00  INFO 21708 --- [relational-data-access] [           main] c.e.f.r.RelationalDataAccessApplication  : Inserting customer record for Josh Long
2024-03-15T11:49:26.304+01:00  INFO 21708 --- [relational-data-access] [           main] c.e.f.r.RelationalDataAccessApplication  : Querying for customer records where first_name = 'Josh':
2024-03-15T11:49:26.320+01:00  INFO 21708 --- [relational-data-access] [           main] c.e.f.r.RelationalDataAccessApplication  : Customer[id=3, firstName='Josh', lastName='Bloch']
2024-03-15T11:49:26.321+01:00  INFO 21708 --- [relational-data-access] [           main] c.e.f.r.RelationalDataAccessApplication  : Customer[id=4, firstName='Josh', lastName='Long']
2024-03-15T11:49:26.324+01:00  INFO 21708 --- [relational-data-access] [ionShutdownHook] com.zaxxer.hikari.HikariDataSource       : HikariPool-1 - Shutdown initiated...
2024-03-15T11:49:26.326+01:00  INFO 21708 --- [relational-data-access] [ionShutdownHook] com.zaxxer.hikari.HikariDataSource       : HikariPool-1 - Shutdown completed.
[..]
```

## TODO

* Deal with the different tasks presented in the issues in the right order.

## Licence

The repo is based on official sample provided by [the Spring Relational Data Access Sample](https://spring.io/guides/gs/relational-data-access)