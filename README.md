# Consumer-Driven Contract Tests

Example of how we can test REST API contract between consumer and provider (popular in microservices architecture where 
there are no dependencies between apps). First solution is ofc E2E testing, but there is simpler idea - contract testing.

[Pact](https://docs.pact.io/readme) is a contract testing tool. 
Contract testing is a way to ensure that services (such as an API provider and a client) 
can communicate with each other. Without contract testing, the only way to know that services can communicate is by using 
expensive and brittle integration tests.

This example consists of consumer `consumer-angular-app` (REST API client) and provider `provider-springboot-app` (REST API provider)

## How it works

Consumer is providing input to interface. Then calls provider and the test asserts if the results meet the expectations defined in contract.

### Pact Broker - repository for pacts contracts
[Pact Broker](https://github.com/pact-foundation/pact_broker) is a tool that is used as artifact repo with versioned pact contracts.
* https://pawelchrzaszczewski.pact.dius.com.au
* Username (read only): VpbbV82mi8DL8Dw9SbOOlpuxF4NJc0
* Password (read only): sXSEuvhHpRH1S9aVDUZrTdmt4XQ7Z


