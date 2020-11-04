1. Run devstart
2. Open localhost:5000/graphql


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


```javascript
{
  books {
    id
    name
    author {
      id
      name
    }
  }
}
```

```javascript
query{
  authors{
    id
    name
    books{
      id
      name
    }
  }
}
```

```javascript
mutation{
	addBook(name:"test book" authorId: 123){
    authorId
  }
}
```

```javascript
mutation{
	addAuthor(name:"test author 12345"){
    name
  }
}
```
