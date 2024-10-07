# Generate clean and comprehensive component tests

⏰ WIP, draft, writing now during October

## Test template and practices

Here is an example of a well-written test

1. The test title should have the pattern of 'When... then'

TBD soon


## Which tests to generate

For each route in the provided OpenAPI, generate the following test cases:

1. Happy path - Provide valid values, ensure the result schema and status are as described in the OpenAPI
2. Each possible response - For each documented HTTP status response, please include a test that simulates the condition to trigger this response and assert that indeed the right response is returned
3. Bad request body - For each mandatory field, create a test that assign invalid value in this field and assert for the corresponding documented error (e.g., http status 400)
4. Unauthorized test - If the route has a security schema, call it with a valid payload but compromise the security requirements and expect to get 401 or 403, based on the spec
5. The new state - If a post route, ensure that the new state is as expected. For example, if a new record is likely to be added, query for that new record and ensure that it matches the incoping payload
6. If you have other ideas not listed below, only if they are highly valuable, include these in a dedicated section 'Other ideas'
_5. 20 other instructions soon_
