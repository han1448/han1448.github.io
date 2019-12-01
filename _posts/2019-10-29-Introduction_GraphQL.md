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