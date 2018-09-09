# Angular Consumer Pact

Example how create [Pact](http://pact.io) files from a consumer test and validate the
a consumer against the Pact.

## How to Run

Run `npm install` to load the needed javascript libraries and then `npm run test` to
run the tests. After the tests have successfully run the created pact file will be
created in the folder `pacts`. 

Then, you can call `npm run publish-pacts` to publish the pact files to a [Pact Broker](https://github.com/pact-foundation/pact_broker).
Need to provide access details: host, user, password (publish-pacts.js).
