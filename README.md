# Library_API
This was the first time creating the API in Golang for me during my learning of the language and it is about the library which contains books for easier communication between server and client of the library.

We need to have the Golang installed into our system and we can just run the code as,
```
$ go run first.go
```

After execution of the Golang file, we can perform various requests either GET, POST or any other and the method of performing the request can be found in the source code of the file which are also visible here as using the CURL for the making of the request to the API,

```
GET
$ curl localhost:8080/books

POST
$ curl localhost:8080/books --include --header "Content-Type: application/json" -d @body.json --request "POST"

Product by ID
$ curl localhost:8080/2 (if the id is 2)

For Checkout/Purchase
$ curl localhost:8080/checkout?id=2 --request "PATCH"

For return/Restock
$ curl localhost:8080/return?id=2 --request "PATCH"
```

> Date of Creation: 2022 April 23 by Rohan Thapa
