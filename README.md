Create a User:
curl -X POST "http://localhost:8080/users" -H "Content-Type: application/json" -d '{"name":"John Doe","email":"john@example.com"}'

Get the User:
curl http://localhost:8080/users/1
(Get user again and see response time.)

Update User:
curl -X PUT "http://localhost:8080/users/1" -H "Content-Type: application/json" -d '{"name":"John Smith","email":"john.smith@example.com"}'

Delete User:
curl -X DELETE "http://localhost:8080/users/1"

Evict All Cache:
curl -X DELETE "http://localhost:8080/users/cache"
