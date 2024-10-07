# Generate clean and comprehensive component tests

⏰ WIP, draft, writing now during October

## Test template and practices

Here is an example of a well-written test

TBD soon


## Which tests to generate

For each route in the provided OpenAPI, generate the following test cases:

1. Happy path - Provide valid values, ensure the result schema and status are as described in the OpenAPI
2. Unauthorized test - If the route has a security schema, call it with a valid payload but compromise the security requirements and expect to get 401 or 403, based on the spec
3. The new state - If a post route, ensure that the new state is as expected. For example, if a new record is likely to be added, query for that new record and ensure that it matches the incoping payload
_4. 20 other instructions soon_
