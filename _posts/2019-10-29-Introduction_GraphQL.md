---
layout: post
title: Kotlin JUnit Test
tags: [ junit, spring]
author-id: oppalove
excerpt_separator: <!--more-->
---
# Overview
GraphQL is a query language for your API, and a server-side runtime for executing queries 
by using a type system you define for your data.

 <!--more-->
 
 A GraphQL service is created by defining types and fields on those types, 
 then providing functions for each field on each type. 
 
 ```:json
type Query {
  me: User
}

type User {
  id: ID
  name: String
}
 ```

Along with functions for each field on each type
```javascript
function Query_me(request) {
  return request.auth.user;
}

function User_name(user) {
  return user.getName();
}
```

Once a GraphQL service is running (typically at a URL on a web service), it can be sent GraphQL queries to validate and execute. 
A received query is first checked to ensure it only refers to the types and fields defined, then runs the provided functions to produce a result.

For example the query:
```json
{
  me {
    name
  }
}
```

Could produce the JSON result:
```json
{
  "me": {
    "name": "Luke Skywalker"
  }
}
```

