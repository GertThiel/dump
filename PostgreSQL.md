# PostgreSQL

[PostgreSQL most useful extensions](http://railsware.com/blog/2012/04/23/postgresql-most-useful-extensions/)

Search for
["postgres" at Github](https://github.com/search?q=postgres&repo=&langOverride=&start_value=1&type=Repositories&language=Ruby)

## Backup ##

Heroku's [WAL-E](https://github.com/heroku/WAL-E)


## Ruby, Rails ##

[Rails on PostgreSQL](http://railsonpostgresql.com/) weblog

[activerecord-postgresql-arrays](https://github.com/funny-falcon/activerecord-postgresql-arrays)
- PostgreSQL array awarness for ActiveRecord

[activerecord-postgres-uuid](https://github.com/ivanvanderbyl/activerecord-postgres-uuid)
adds support for the 128 bit [UUID](http://www.postgresql.org/docs/current/static/uuid-ossp.html)
column type to ActiveRecord

[enum_type](https://github.com/RISCfuture/enum_type)
— enumerated types in ActiveRecord

<del>[has\_metadata\_column](https://github.com/RISCfuture/has_metadata_column)
reduce table width and migration overhead by moving non-indexed columns to a
separate metadata column</del>

[hierarchy](https://github.com/RISCfuture/hierarchy) lets you use
[LTREE](http://www.postgresql.org/docs/current/static/ltree.html)-utilizing hierarchies in ActiveRecord

[pg_comment](https://github.com/albertosaurus/pg_comment)
adds PostgreSQL comment support to Rails migrations

[postgresql-cursor](https://github.com/afair/postgresql-cursor) is an extension
to the ActiveRecord PostgreSQLAdapter for very large result sets. It provides a
cursor open/fetch/close interface to access data without loading all rows into
memory, and instead loads the result rows in “chunks” (default of 10.000 rows),
buffers them, and returns the rows one at a time.

[queue_classic](https://github.com/ryandotsmith/queue_classic)
is a worker queue for Ruby applications that uses unbelievably awesome features in PostgreSQL

[transaction_retry](https://github.com/qertoip/transaction_retry) retries
database transaction on deadlock and transaction serialization errors

## PostgreSQL as a document store for schemaless data ##

### Hstore ###

[activerecord-postgres-hstore](https://github.com/softa/activerecord-postgres-hstore)

### JSON ###

…

The JSON column type and [PLV8](https://code.google.com/p/plv8js/)

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

The Homebrew formular for [PLV8](https://code.google.com/p/plv8js/) at
[will/homebrew](https://github.com/will/homebrew/commit/0053e3b78bf36d20822a6da966064c905bb3c4b4)
could be a blueprint for my `smlar` formular
([Formula Cookbook](https://github.com/mxcl/homebrew/wiki/Formula-Cookbook)).
