# Learn-GraphQL

## Set up server
- npm install

## Start server
- npm run devStart

## Example Queries
```
// query data
query {
  author(id: 1) {
    id
    name
  }
}

// query data
query {
  book(id: 1) {
    id
    name
  }
}

// query data
query {
  books {
    id
    name
    author {
      id,
    }
    
  }
}

// query data
query {
  books {
    id
    name
    author {
      id,
    }
  }
}

// edit data
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
