```
    Spring vs Spring Boot
```
#   [Spring]
#   [1] enterprise level java apps
#   [2] dependency injection [inversion of control] []
#   [3] largely manual configurations (XML, annotations)
#   [4] more boilerplate code
#   [5] set up server and deployment descriptor explicitly


#   [Spring Boot] []
#   [1] built on top of Spring framework
#   [2] build standalone, production ready apps
#   [3] auto-configuration, reduces boilerplate code
#   [4] starter dependencies to manage project dependencies
#   [5] embedded server for easy deployment


#   [Spring vs Spring Boot] []
#   [configuration] Spring requires more manual configuration, Spring boot auto-configured
#   [dependency management] [] Spring needs manual dependency definition, Spring Boot uses 'starter' dependencies
#   [embedded server] [] Spring apps need separate server, Spring boot has embedded server
#   [Rapid development] [] faster app developement as compared to Spring
#   [use-cases] [] Spring suited for large, enterprise apps, Spring Boot to build microservices and standalone apps



```
    Spring Security
```

#   [Authentication and Authorization] [] 
#   [Protection against attacks] []
#   [Java servlet api integration to secure web apps] []
#   [Spring MVC integration] []
#   [Extensibility]
#   [Thymeleaf integration] [] integrates well with Thymeleaf template engine, providing a special thymeleaf dialect for expressing security constraints in views.



```
    Spring Boot Architecture
```

#   [Presentation layer] [] [1] handles HTTP requests and performs authentication, [2] converts JSON to java objects and vice-versa, [3] Passes authenticated requests to business layer

#   [Business layer] [] [1] contains app's business logic, [2] performs validation and authorization, [3] interacts with persistence layer

#   [Persistence layer] [] [1] manages storage logic including database operations, [2] Translates b/w database rows and business objects, [3] communicates with database layer

#   [Database layer] [] [1] Represents actual database used by the application, [2] has databases like MySQL, MongoDB etc. [3] performs CRUD operations

#   [DAO layer] [] sits b/w service layer and database layer, responsible for interacting with databases. [1] Repository interface [::] implemented using repository interface, which extends the Spring Data JPA 'ÇrudRepository' interfaces for CRUD operations, [2] Entity mapping [::] associated with entity classes that map to database tables, annotated with JPA annotations [@Table], [@Column] etc.. [3] Query Methods [::] define custom query methods, [4] transaction management [::] to manage db transactions ensuring database consistency and integrity, [5] error handling [::] handle and  translate db-specific exceptions into app-level exceptions, [6] testability [::] without setting up entire app context dao layer can be tested in isolation.



#   [antmatchers] [] this method allows to specify URL patterns to match when configuring security constraints



#   [Spring Boot components] [] 
#   [controllers] defined in presentation layer, handle incoming HTTP requests and responses,
#   [services] defined in business layer, encapsulates app's core logic and business rules
#   [repository/DAO] defined in persistence layer, handle data access and database operations.
#   [entities] defined in persistence layer, represent data model and map to database table
#   [Data Transfer Objects --- DTOs] []  To transfer data between layers, avoiding direct exposure to internal data structures.