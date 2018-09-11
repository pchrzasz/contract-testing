# Springboot Contract Provider

Basing on CDC (consumer-driven contract).

During every `./gradlew build` contract is downloaded from Pact Broker (remote contract repository - done by gradle task `downloadFile`) 
and JUnit tests validating controller against contract are generated (by Spring Cloud Contract Gradle plugin) in 
dir: `build/generated-test-sources/contracts/org/springframework/cloud/contract/verifier/tests/` and executed.

`./gradlew clean` cleans directory with retrieved contracts from Pact Broker: `provider-springboot-app/src/test/resources/contracts/userservice`.

Key files:
* UserController (REST controller)
* UserServiceBase (abstract class which will be inherited in generated JUnits)