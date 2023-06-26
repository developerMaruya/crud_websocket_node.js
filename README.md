crud using web socket in node.js

ws://localhost:3000  // connect

after connect hit

// create........................

body- {
  "type": "register",
  "username": "vishal",
  "password": "vishal",
  "email": "vishal@example.com",
  "mobile": "1234567890",
  "role": "user"
}
// send
output-
{"id":16}
{ "type": "register", "username": "vishal", "password": "vishal", "email": "vishal@example.com", "mobile": "1234567890", "role": "user" }
17:21:26
Connected to ws://localhost:3000


// updage ....
body-
{
  "type": "updateEmployee",
  "username": "vishal",
  "password": "vishal",
  "email": "vishal1@example.com",
  "mobile": "1234567890",
  "role": "user"
}
output-
{"message":"Employee details updated"}
{ "type": "updateEmployee", "username": "vishal", "password": "vishal", "email": "vishal1@example.com", "mobile": "1234567890", "role": "user" }

// get..............
body-
{
  "type": "getEmployee",
  "username": "vishal",
  "password": "vishal"
}
output-
{"id":16,"username":"vishal","email":"vishal1@example.com","mobile":1234567890,"role":"user"}
{ "type": "getEmployee", "username": "vishal", "password": "vishal" }

// delete....................
body-
{
  "type": "deleteEmployee",
  "username": "vishal",
  "password": "vishal"
}
output-
{"message":"Employee deleted"}
{ "type": "deleteEmployee", "username": "vishal", "password": "vishal" }