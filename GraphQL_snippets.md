GraphQL  in a Nutshell:
--------
    * queries and mutations
    * schemas and types

    Query:
        - fields
        - arguments
        - aliases

    Queries:
        - variables
        - fragments // are like spread operator in JS
        - directives

    Mutations:
        used for create, update, delete

    Schemas and simple types:
        - scalar
        - imput
        - types
            ! means that the field is required
            ID type is just a scting

    Complex types:
        - enum 
        - interface
        - union : which will resolve to some of the mentioned types
        - type which 'implements' already defined interfaces

    Gotchas:
        - N+1
        - caching is hard:
            -recomende client cache
            - bad get request
            - think redux / reselect memorization
            - server side batching
        really easy to hamemr a DB if not careful
