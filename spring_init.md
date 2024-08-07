```
    Spring features
```
#   [auto-configuration] auto import depedencies in pom.xml [maven-build]
#   [stand-alone app] [] no need for separate application server, app can be run from cli

#   [opinionated defaults] [] reduced boilerplate code
#   [embedded server] [] tomcat, jetty, undertow

#   [spring-boot-starters] [] spring-boot-starter-web includes all necessary dependencies required to create web app

#   [spring boot cli] [] cli tool to run groovy scripts, quick prototype spring apps

#   [microservices architecture] [] to build microservices apps,


#   [spring boot actuator] [] monitor app code

#   [external configuration] [] use properties files, yaml files, environment variables, cli args

#   [devTools] [] for enhancing dev experience, automatic restarts, live reload, configs for easier debugging

#   [SpringApplication] launches spring application from Java main method, sets up default configuration and starts spring application context.

#   [annotations] to help identify reserved code blocks
#   [@SpringBootApplication] includes [@Configuration], [@EnableAutoConfiguration], [@ComponentScan], 

#   [@Configuration] source of bean definitions, 
#   [@EnableAutoConfiguration] tells Spring Boot to start adding beans based on classpath settings, other beans and various property settings.
#   [@ComponentScan] Tells Spring to look for other components, configurations and services in the specified package.

#   [@RestController] Combines [@Controller] and [@ResponseBody], simplifies creation of RESTful web services
#   [@RequestMapping] Maps HTTP requests to handler methods of MVC and REST controllers.

#   [Application properties (application.properties/*.yaml)] [] to specify server port, database configurations and other settings.

#   [Profiles] [] Spring Boot supports different profiles for different developments (development, testing, production), [@Profile] specifies beans that should only be loaded for specific profiles

#   [health checks and metrics] [] Spring Boot actuator monitors and manages app, includes endpoint for health checks('/actuator/health'), metrics ('/actuator/metrics')


#   [IoC --<>-- Inversion of Control] [] resposible for instantiating, [configuring] and [assembling] spring beans in app

#   [configuring beans] [] define custom beans using [@Configuration] and [@Bean]

#   [Component Scanning] [] scans for [@Component] [@Service], [@Repository] [@Controller] and registers them as beans in IoC container


#   [@Component] [1] marks a class as a bean, [2] spring registers component classes as bean in IoC container, [3] dependency injection, [4] bean name same as class name with 1st letter in lower case, 

#   [Property binding] [] binds environment properties to bean properties to easily configure beans using application.properties



#   [Implementations of IoC container] [] 
#   [Bean Factory] [] provides configuration framework and basic functionality to manage beans
#   [ApplicationContext] BeanFactory subinterface adds more enterprise specific functionality, easier integration of Spring's AOP features, [message resource handling] [] and [event publication] []

#   Spring Boot simplifies IoC container configuration by providing : 
#   [Auto-configuration] automatically configures IoC container based on app dependencies.
#   [Starter-dependencies] reduce amount of manual configuration 
#   [embedded-server] embeds Tomcat, Jetty, undertow server directly in app

#   


#   [Dependency Injection] [] done in following way : 
#   [auto-configuration] automatically configures IoC container based on dependencies in classpath, reduces amount of manual configuration
#   [starter dependencies] [] pulls in necessary dependencies and their transitive dependencies, reduces configuration
#   [constructor injection] [] favors constructor injection over [setter injection] [] promoting immutable, thread-safe objects, avoids need for boilerplate setter methods

#   [constructor injection] [] setting up required objects in constructor rather than in setter method

#   [AOP ---<>--- Aspect Oriented Programming] []
#   to add additional behavior to existing code without modifying original code. 
#   [Advice types] [] [@Before, @After, @AfterReturning] [] to execute custom logic at different points in method execution.


#   [spring web] [] for java based web apps, 

#   [spring security] [] powerful, customizable authentication, access-control framework, [features...]
#   [authentication] provides support for authenticating users including OAuth2.0
#   [authorization] secure web requests, methods, domain objects
#   [protection against attacks] [] protect common web app attacks like cross-site forgery
#   []