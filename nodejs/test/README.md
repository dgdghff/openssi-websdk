# Testing openssi-websdk

A mocha test suite is provided for integration testing as well as to document common self-sovereign identity steps.

## Configuration

1. To execute the tests, manually create agents for the following roles: holder, issuer, verifier.
2. Inside the `nodejs` directory, create a `.env` file with the following properties related to the agents you created.

```env
ACCOUNT_URL=
ADMIN_NAME= Julie Pena
ADMIN_PASSWORD= cloe
ISSUER_AGENT_NAME= Valerie Garcia 
ISSUER_AGENT_PASSWORD= lonlon
HOLDER_AGENT_NAME= cassandra hernandez
HOLDER_AGENT_PASSWORD= babymaggie3
VERIFIER_AGENT_NAME= madeline 
VERIFIER_AGENT_PASSWORD= melvin
```

The `ACCOUNT_URL` can be obtained from the browser's address bar when accessing the agency dashboard. It will appear similar to `https://<guid>.<subdomain>.containers.appdomain.cloud`.

The `ADMIN_NAME` and `ADMIN_PASSWORD` is the name and password of the first agent you create.

Agent names and passwords can be seen on the **Add Device** -> **Manual Entry** screen.

## Running

From the `nodejs` directory, execute `npm test`.
