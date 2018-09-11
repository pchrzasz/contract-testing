# Consumer-Driven Contract Tests

Example of how we can test REST API contract between consumer and provider (popular in microservices architecture where 
there are no dependencies between apps). First solution is ofc E2E testing, but there is simpler idea - contract testing
executed during integration tests.

An integration test is a test between an API provider and an API consumer that asserts that the provider returns expected 
responses for a set of pre-defined requests by the consumer. 
The set of pre-defined requests and expected responses is called a contract.

This example consists of consumer (`consumer-angular-app`) - application written using Angular JS and provider (`provider-springboot-app`) - app written in Java.

## How it works

Consumer is providing input to interface. Then calls provider and the test asserts if the results meet the expectations defined in contract.

