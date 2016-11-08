# Diesel ODBC Driver

It is highly underdevelopment! Unstable API warning! I will tell when it is ready.

It started from a need of odbc in one of my projects, at that time I was using Diesel.

## TODO
- Implementation of the Connection trait.
- Implementation of the Backend.
- Implementation of the query builder.
- Implementation of the bind collector.
- If the data is transmitted in a non-standard format, it'll need to provide ToSql and FromSql impls for the various types
- Sample can be found for the pg implementation here: https://github.com/diesel-rs/diesel/tree/master/diesel/src/pg.
It's the simplest, but we also have stuff in there for PG specific types and expressions.
sqlite is here https://github.com/diesel-rs/diesel/tree/master/diesel/src/sqlite,
which has no backend specific types or expressions but does have a more involved backend
implementation as it has it's own API for data fetching
