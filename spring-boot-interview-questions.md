**Part 1**
1. What is Spring Boot?
A framework that simplifies Spring development using auto-configuration, embedded servers, and starter dependencies.

2. Why use Spring Boot?
Fast development, minimal configuration, embedded Tomcat/Jetty, auto-config, and starter dependencies.

3. What is auto-configuration?
Spring Boot automatically configures beans based on classpath and properties.

4. What are Spring Boot Starters?
Predefined dependencies that reduce manual version management.
Example: spring-boot-starter-web, spring-boot-starter-data-jpa.

5. Difference between Spring and Spring Boot?
Spring → Requires manual config.
Spring Boot → Auto-config + embedded server + starters.

6. What is Spring Boot Actuator?
Provides production-ready endpoints like /health, /metrics, /info.

7. How to enable Actuator?
Add dependency: spring-boot-starter-actuator.

8. What is Spring Boot CLI?
Command-line tool to run Groovy scripts quickly.

9. What is Spring Initializr?
Online generator to create Spring Boot project structures.

10. What is @SpringBootApplication?
Meta-annotation combining @Configuration, @EnableAutoConfiguration, @ComponentScan.

11. What is @RestController?
Combines @Controller + @ResponseBody to return JSON directly.

12. How do you create a REST API?
Use @RestController + @GetMapping / @PostMapping.

13. What is @RequestMapping?
Maps HTTP requests to methods.

14. Difference between @GetMapping and @PostMapping?
@GetMapping → Read data
@PostMapping → Create data

15. Purpose of application.properties?
Externalized configuration: DB, port, logging, etc.

16. How to change server port?
server.port=8081

17. Difference between JPA and Hibernate?
JPA → Specification
Hibernate → Implementation of JPA

18. What is an embedded server?
Built-in Tomcat/Jetty that runs inside the application. No external server needed.

19. How do you handle exceptions?
Use @RestControllerAdvice and @ExceptionHandler.

20. What is Spring Boot DevTools?
Provides auto-restart and live reload during development.

21. What is Spring Security?
Framework for authentication and authorization.

22. What are Spring Profiles?
Environment-specific configs (dev, test, prod).
Activate using: spring.profiles.active=dev

23. What is caching in Spring Boot?
Use @EnableCaching, @Cacheable, @CacheEvict to store method results.

24. How to schedule tasks?
Use @EnableScheduling + @Scheduled.

25. What is CommandLineRunner?
Runs code immediately after startup.

26. Difference between @Component, @Service, @Repository?
All are beans but used for semantic roles:
@Component → generic
@Service → business logic
@Repository → DB layer + exception translation

27. How to run Spring Boot as a JAR?
Build: mvn clean install
Run: java -jar app.jar

28. What is @ConfigurationProperties?
Binds external config into POJO.

29. What is SpringApplication.run()?
Starts the application, loads context, initializes beans, and starts embedded server.

30. How to connect to a database?
Configure spring.datasource.url, username, password, and JPA properties.

**Part 2**

31. What is the difference between @ComponentScan and @Component?
@ComponentScan → tells Spring where to search for beans.
@Component → marks a class as a Spring bean.

32. What is the purpose of @Bean?
Manually declare a bean in a @Configuration class.

33. What is Spring Boot Starter Test?
A testing starter providing JUnit, Mockito, Spring Test, JsonPath, etc.

34. How to enable asynchronous methods?
Use @EnableAsync + @Async.

35. What is @Transactional?
Ensures a method runs inside a database transaction.

36. What is the difference between @PathVariable and @RequestParam?
@PathVariable → part of URI.
@RequestParam → query parameters.

37. What is the use of ModelMapper or MapStruct?
For mapping DTOs to entities and vice-versa.

38. What is H2 Database?
In-memory database commonly used for local development and testing.

39. What is the purpose of application.yml?
Same as application.properties but allows hierarchical YAML structure.

40. What is Flyway or Liquibase?
Database migration tools used to version and manage DB schema.

41. What is @Value annotation?
Injects values from properties/yaml into variables.

42. What is Spring Cloud Config?
Externalized configuration stored in Git, server used to serve configs to multiple services.

43. What is Feign Client?
A declarative HTTP client used in microservices to call other services easily.

44. What is RestTemplate?
Traditional Spring client to make HTTP calls (now replaced by WebClient).

45. What is WebClient?
Reactive, non-blocking HTTP client used in Spring WebFlux and modern apps.

46. What is the purpose of @EnableEurekaClient?
Registers the service with Eureka service discovery.

47. What is Resilience4j?
Library for circuit breaker, retry, rate limiting, bulkhead patterns.

48. How to configure logging?
Using application.properties or logback-spring.xml.

49. What is Actuator's /health endpoint used for?
To check if the application is running — used by load balancers and Kubernetes.

50. What is a fat JAR in Spring Boot?
A self-contained jar that includes application + all dependencies + embedded server.

51. What is a microservice in Spring Boot?
A small, independent service owning one business function, built using Spring Boot.

52. What is the difference between Monolithic and Microservices architecture?
Monolithic → One big application.
Microservices → Many small, independent services communicating via REST/Kafka.

53. What is load balancing in Spring Cloud?
Distributing requests across multiple service instances using Ribbon, Spring Cloud LoadBalancer, or Gateway.

54. What is Swagger/OpenAPI?
Tool to generate API documentation and interactive UI for testing endpoints.

55. How do you enable Swagger in Spring Boot?
Add springdoc-openapi dependency and access /swagger-ui.html.

56. What is CORS and how to enable it?
Cross-Origin Resource Sharing — allows frontend apps to call APIs.
Enable using @CrossOrigin.

57. What is Multipart in Spring Boot?
File upload handling done using MultipartFile.

58. What is the difference between @RequestBody and @ResponseBody?
@RequestBody → Convert JSON → Java object
@ResponseBody → Convert Java → JSON

59. What is an interceptor in Spring Boot?
A component used to intercept requests before they reach the controller (logging, auth, etc.).

60. What is a filter in Spring Boot?
A Servlet-based component used for request/response processing at a lower level (security, logging).

**Part 3**
