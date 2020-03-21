# Learn-GraphQL

## Set up server
- npm init
- npm i express express-graphql graphql
- npm install --save-dev nodemon

## Start server
- npm run devStart

## Example Queries
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
