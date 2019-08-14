# terminus-ontologies
Terminus DB Ontologies

The Terminus Ontologies are a self-documenting, formal description of all of the internal datatypes and classes used by the Terminus DB egnine. They cover such aspects as documents, relationships, time and space and geo-temporal scoping of data and values. Annotations and provenance and a range of basic building blocks such as new and useful datatypes and classes.  

On top of these core ontologies, the terminus DB ontologies define the governance structure of the dataase itself - they form the schema of the capability database that governs the system itself. It's ontologies all the way down - every part of the server's configuration and saved state has a schema managed by the system, even the capability database. It's ontologies all the way down, we eat our own dogfood! This makes a lot of sense because we get user-interfaces and forms for free if we use our own system. Using ontologies to describe the internal datatypes and structures allows us to much more easily extend and improve our system as we learn more. 

The specific ontologies and how they are used by Terminus DB are detailed below. 
