# entity-service

this is a work in progress project to create an architecture for micro-services operating on data entities where specification is decoupled from implementation.

## influences

- http://www.confreaks.com/videos/759-rubymidwest2011-keynote-architecture-the-lost-years
- TODO

## concepts

### entity

an entity is a collection of data, like the properties of a class.

### entity schema

an entity schema is a description of an entity that describes the properties' expected structure and values.

### service

a service is a collection of functions, like the methods of a class.

### service spec

a service spec is a description of a service that describes the methods' expected input and output entities.

### service detail

a service detail is an implementation of a service that provides the methods' function.

### service block

a service app is a combination of a service spec and a service detail.

### service interface

a service interface connects services that abide to specific service specs to be available over external details, such as HTTP or WebSockets.

## expected process

entity schema -> SCRUD service spec

entity schema -> SCRUD service detail

SCRUD spec + SCRUD db detail = SCRUD block

SCRUD block + SCRUD interface = SCRUD app
