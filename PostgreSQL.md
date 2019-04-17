# PostgreSQL

[PostgreSQL most useful extensions](http://railsware.com/blog/2012/04/23/postgresql-most-useful-extensions/)

Search for
["postgres" at Github](https://github.com/search?q=postgres&repo=&langOverride=&start_value=1&type=Repositories&language=Ruby)

## Backup ##

[Barman](http://www.pgbarman.org): disaster recovery for business critical PostgreSQL databases

Heroku's [WAL-E](https://github.com/heroku/WAL-E)


## GraphQL ##

[Graphile](https://www.graphile.org/)
(Javascript, Node.js)

[Hasura](https://hasura.io/)
(Haskell)

[Graphile vs Hasura?](https://www.reddit.com/r/graphql/comments/a84s22/graphile_vs_hasura/)

> PostGraphile is written in JavaScript which is more approachable than Hasura’s Haskell …

[PostgREST](http://postgrest.org/) (Haskell)
is a standalone web server that turns your PostgreSQL database directly into a
RESTful API. The structural constraints and permissions in the database determine
the API endpoints and operations

<del>[Prisma](https://www.prisma.io/),
successor of [Graphcool](https://www.graph.cool/)</del>


## OLAP ##

[Basic OLAP Support in PostgreSQL 9.5](http://www.thatguyfromdelhi.com/2015/05/basic-olap-support-in-postgresql.html)


## Ruby, Rails ##

[Rails on PostgreSQL](http://railsonpostgresql.com/) weblog

[activerecord-postgresql-arrays](https://github.com/funny-falcon/activerecord-postgresql-arrays)
- PostgreSQL array awareness for ActiveRecord

[activerecord-postgres-hstore](https://github.com/engageis/activerecord-postgres-hstore):
Goodbye serialize, hello hstore. Speed up hashes in the database

[activerecord-postgres-hstore-core](https://github.com/jtvjt/activerecord-postgres-hstore-core)

[activerecord-postgres-uuid](https://github.com/ivanvanderbyl/activerecord-postgres-uuid)
adds support for the 128 bit [UUID](http://www.postgresql.org/docs/current/static/uuid-ossp.html)
column type to ActiveRecord

[dagnabit](http://gitorious.org/dagnabit) is an ActiveRecord plugin for
directed acyclic graphs. It stores directed acyclic graphs as an adjacency
list, using recursive common table expressions to perform fast reachability
queries

[enum_type](https://github.com/RISCfuture/enum_type)
— enumerated types in ActiveRecord

[has\_metadata\_column](https://github.com/RISCfuture/has_metadata_column)
reduce table width and migration overhead by moving non-indexed columns to a
separate metadata column

[hierarchy](https://github.com/RISCfuture/hierarchy) lets you use
[LTREE](http://www.postgresql.org/docs/current/static/ltree.html)-utilizing
hierarchies in ActiveRecord

[partitioned](https://github.com/fiksu/partitioned): PostgreSQL database table
partitioning support for Rails

[pg_comment](https://github.com/albertosaurus/pg_comment)
adds PostgreSQL comment support to Rails migrations

[pg_search](https://github.com/Casecommons/pg_search) builds ActiveRecord
named scopes that take advantage of PostgreSQL's full text search

[postgresql-cursor](https://github.com/afair/postgresql-cursor) is an extension
to the ActiveRecord PostgreSQLAdapter for very large result sets. It provides a
cursor open/fetch/close interface to access data without loading all rows into
memory, and instead loads the result rows in “chunks” (default of 10.000 rows),
buffers them, and returns the rows one at a time.

[postgres_ext](https://github.com/dockyard/postgres_ext) adds support for
missing PostgreSQL data types to ActiveRecord: Arrays, CIDR, INET, MACADDR,
UUID

[queue_classic](https://github.com/ryandotsmith/queue_classic)
is a worker queue for Ruby applications that uses unbelievably awesome features in PostgreSQL

[silent-postgres](https://github.com/dolzenko/silent-postgres) silences
PostgreSQL connection adapter verbose output

[switcheroo](https://github.com/moneydesktop/switcheroo): ActiveRecord
migration library to speed up schema changes for large PostgreSQL tables

[transaction_retry](https://github.com/qertoip/transaction_retry) retries
database transaction on deadlock and transaction serialization errors

## PostgreSQL as a document store for schemaless data ##

### Graph ###

[AgensGraph](http://www.agensgraph.com/),
[GitHub](https://github.com/bitnine-oss/agensgraph),
© Apache-2.0

### Hstore ###

[activerecord-postgres-hstore](https://github.com/engageis/activerecord-postgres-hstore)

[hstore_flags](https://github.com/infinitysw/hstore_flags) stores boolean flags
in a PostgreSQL hstore field

[multilang-hstore](https://github.com/firebaseco/multilang-hstore) is a small
library for translating database values for Rails 3 and PostgreSQL hstore

### JSON ###

…

The JSON and JSONB column types and [PLV8](https://code.google.com/p/plv8js/)

### Time-Series ###

[TimescaleDB](https://www.timescale.com/),
[GitHub](https://github.com/timescale/timescaledb),
© Apache-2.0

### XML ###

…

## Full Text Search ##

…

## Local Check for Plagiarism ##

[Effective similarity search in PostgreSQL](http://railsware.com/blog/2012/05/10/effective-similarity-search-in-postgresql/)
using
[smlar](http://sigaev.ru/git/gitweb.cgi?p=smlar.git;a=blob;hb=HEAD;f=README)
which calculates similarity of arrays for PostgreSQL 9.1+

    git clone git://sigaev.ru/smlar

or [ssdeep_psql](https://github.com/bernerdschaefer/ssdeep_psql)

The Homebrew formular for [PLV8](https://code.google.com/p/plv8js/) at
[will/homebrew](https://github.com/will/homebrew/commit/0053e3b78bf36d20822a6da966064c905bb3c4b4)
could be a blueprint for my `smlar` formular
([Formula Cookbook](https://github.com/mxcl/homebrew/wiki/Formula-Cookbook)).
