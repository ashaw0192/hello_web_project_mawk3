GET /names Route Design Recipe

1. Design the Route Signature

method: POST
path: /sort-names
body: string of names seperated by commas

2. Design the Response

# With body parameters
names=Joe

# expected response
Joe

# With body parameters
names=Joe,Alice,Zoe,Julia,Kieran

# expected response
Alice,Joe,Julia,Kieran,Zoe

3. Write Examples

# Request:

POST /sort-names?names=Joe

# Expected response:

Response for 200 OK

# Request:

POST /sort-names?names=Joe,Alice,Zoe,Julia,Kieran

# Expected response:

Response for 200 OK

4. Encode as Tests Examples

5. Implement the Route
