# graphql-sample-app (WIP)
[GraphQL](http://www.graphql.org/) is an API standard that provides a more efficient, powerful and flexible alternative to REST.

This is a sample app to create GraphQL server using following technologies:
- `graphql-yoga` :
  - GraphQL server which is built on top of [Express](https://expressjs.com/), `apollo-server`,`graphql-js`
- [Prisma](https://www.prisma.io/)
  - Replacement for traditional ORMs. Used to implement GraphQL resolvers and simplify database access by heavy-lifting data-access/mutations in background.
- [GraphQL Playground](https://github.com/prisma/graphql-playground)
  - IDE for GraphQL
  - Auto-generates comprehensive documentation for available API operations
  - Editor to write queries/mutations/subscriptions with auto-complete and syntax-highlighting
  - Can share API operations


###### Adding dependency
- yarn install

###### Deploying on prisma
- prisma deploy

It will deploy the schema to prisma (you need to be logged in to prisma to push the schema changes) and then generates the prisma client through `post-deploy` `hook`

###### Start GraphQL server
- node src/index.js

`GraphQL Playground` can be accessed at [http://localhost:4000/](http://localhost:4000/)
