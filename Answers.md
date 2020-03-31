Tasks
* Configuration Projects use Spring Cloud Configuration. Each service has a configuration in service/src/java/resources/bootstrap.yml. There is URI, from which is configuration obtained (in our case configuration server on localhost:8888).  Configuration server getting configuration from the [git repository](https://github.com/spring-petclinic/spring-petclinic-microservices-config). We can change the target repository or create configuration locally in a file.
* Startup order: depends_on in docker-compose.
* The service wait for others to start: dockerize wait.
