# Terminus DB Ontologies

The Terminus Ontologies are a self-documenting, formal description of all of the internal datatypes and classes used by the Terminus DB egnine. They cover such aspects as internal configuration, documents, relationships, time and space and geo-temporal scoping of data and values, annotations and provenance and a range of basic building blocks such as some useful datatypes and classes.  

On top of these core ontologies, the terminus DB ontologies define the governance structure of the dataase itself - they form the schema of the capability database that governs the system itself. It's ontologies all the way down - every part of the server's configuration and saved state has a schema managed by the system, even the capability database. It's ontologies all the way down, we eat our own dogfood! This makes a lot of sense because we get user-interfaces and forms for free if we use our own system. Using ontologies to describe the internal datatypes and structures allows us to much more easily extend and improve our system as we learn more. 

The specific ontologies and how they are used by Terminus DB are detailed below. 

## terminus - internal state ontology 
terminus.owl.ttl

Contains classes to describe, Agent, User, Role, Capability, Resource, Server, Database and the relationships between them.  

## vio - reasoning violations ontology 
vio.owl.ttl

Contains classes to describe the quality control error messages produced by the system - both schema checks and instance data checks

## documentation - Documentation Ontology 
documentation.owl.ttl

Contains classes to represent the documentation of the system - Content, API & Function Definitions, arguments, types, etc. 

## xdd - Extended Datatypes Ontology
xdd.owl.ttl

Contains 11 extended datatypes which allows use of new datatypes: uncertainty ranges, email, html and json datatypes. 

## dcogbox - Box Ontology 
dcogbox.owl.ttl

Contains wrapper classes for all basic datatypes to support 'boxing' of datatype properties for annotation and qualification.  This is a solution to the problem whereby, in RDF, we cannot directly annotate datatype values (literals). Boxing is a solution to the problem that keeps the integrity of the basic underlying triple format intact. 

## dcog - Core Terminus Ontology 
dcog.owl.ttl

Contains core classes to describe, Document, Entity, Relationship classes, Annotations, Provenance objects, temporal, geographic and geotemporal scopings. Basic building blocks from which sophisticated and complex data structures can be readily constructed. 
