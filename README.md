# hackernews-graphql-java
Project to learn graphql from https://www.howtographql.com/

## Purpose

This is a GraphQL IDE duplicated from graphiql (https://github.com/howtographql/graphql-java/blob/master/src/main/webapp/index.html) for navigating the schema specified in `src/main/resources/schema.graphqls`. 

## Status

This code is completed until step 4 - Connectors (https://www.howtographql.com/graphql-java/4-connectors/)

## Prerequisite

A local Mongo DB instance is required, with a database named 'hackernews'. A collection called 'links' will be created if not available when the program runs.

### Run Mongo DB as a service on OSX

> brew services start mongodb-community@4.4

### Stop Mongo DB running as a service on OSX

> brew services stop mongodb-community@4.4

### To run Mongo DB manually as a background process (Intel)

> mongod --config /usr/local/etc/mongod.conf --fork

### To stop mongod running as a background process, connect to mongod from the mongo shell, and issue the `shutdown` command

Reference
: https://docs.mongodb.com/manual/tutorial/install-mongodb-on-os-x/

## Running 

`mvn jetty:run`

Navigate to `http://localhost:8080`
