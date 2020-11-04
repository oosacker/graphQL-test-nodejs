1. Run devstart
2. Open localhost:5000/graphql
3. Type query { message }
4. Get reponse "Hello World"

Query:
`{
  book(id: 1) {
    id
    name
    author {
      name
    }
  }
}`

Returns:
`{
  "data": {
    "book": {
      "id": 1,
      "name": "Harry Potter and the Chamber of Secrets",
      "author": {
        "name": "J. K. Rowling"
      }
    }
  }
}`