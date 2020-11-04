1. Run devstart
2. Open localhost:5000/graphql

Query:
```javascript
{
  book(id: 1) {
    id
    name
    author {
      name
    }
  }
}
```

Returns:
```javascript
{
  "data": {
    "book": {
      "id": 1,
      "name": "Harry Potter and the Chamber of Secrets",
      "author": {
        "name": "J. K. Rowling"
      }
    }
  }
}
```