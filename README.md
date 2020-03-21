# Learn-GraphQL

## Queries
```
query {
  author(id: 1) {
    id
    name
  }
}

query {
  book(id: 1) {
    id
    name
  }
}

query {
  books {
    id
    name
    author {
      id,
    }
    
  }
}

query {
  books {
    id
    name
    author {
      id,
    }
  }
}

mutation {
  addBook(name: "Super book", authorId: 1) {
    id,
    name
    author {
      name
      books {
        name,
        id
      }
    }
  }
}
```
