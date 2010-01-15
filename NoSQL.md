# Alfresco ECMS

  * [Alfresco](http://www.alfresco.com/),
    [Planet](http://blogs.alfresco.com/planet/),
    [Webcasts](http://blogs.alfresco.com/wp/webcasts/)

# GT.M, M/DB, M/DB:X

  * [GT.M](http://fis-gtm.com) Database Engine with Extreme Scalability and Robustness

  * [M/DB](http://gradvs1.mgateway.com/main/?path=mdb)
    is a Free Open Source "plug-compatible" alternative to
    Amazon's [SimpleDB](http://aws.amazon.com/simpledb/) database

  * [M/DB:X](http://gradvs1.mgateway.com/main/?path=mdbx)
    is a simple, lightweight, yet powerful hybrid JSON/Native XML Database

  * Enterprise Web Developer ([EWD](http://gradvs1.mgateway.com/main/?path=ewd))
    is an advanced web application delvelopment technology and Ajax framework

  * [Using SimpleDB and Rails in No Time with ActiveResource](http://developer.amazonwebservices.com/connect/entry.jspa?externalID=1242)

## Caché

  * InterSystems [Caché](http://www.intersystems.de/cache/) is an advanced
    but commercial 'successor' of GT.M

    Data stored in Caché can be accessed using JDBC and ODBC.

  * Max Lapshin wrote a related [Ruby driver](http://intersys.rubyforge.org/)

# MongoDB

[Why I think Mongo is to Databases what Rails was to Frameworks](http://railstips.org/2009/12/18/why-i-think-mongo-is-to-databases-what-rails-was-to-frameworks)

  * [MongoDB](http://www.mongodb.org/)

  * [Mongoid](http://mongoid.org/)

  * [MongoMapper](http://mongomapper.com/)

GridFS

  * [CarrierWave](http://github.com/jnicklas/carrierwave/)
    supports MongoMapper and offers compatibility to Paperclip

  * [GridFS adapter](http://github.com/retro/gridfs-rackdav) for
    [RackDAV](http://github.com/georgi/rack_dav)

  * [GridFS FUSE](http://github.com/mikejs/gridfs-fuse/) allows you to mount
    a MongoDB GridFS instance as a local filesystem

  * John Nunemaker's fork of [Grip](http://github.com/jnunemaker/grip)
    (from the author of MongoMapper)

  * [Rack::GridFS](http://github.com/skinandbones/rack-gridfs/)

  * [Rails Metal for serving from GridFS](http://github.com/twoism/metal_grid_fs/)

## Install MongoDB

### Mac OS X

    port install mongodb

### Ubuntu

## Install mango\_mapper

Install `mongo_mapper` which will install the MongoDB Ruby driver `mongo`
and `jnunemaker-validatable` as well:

    sudo gem install mongo_mapper

Optionally install `mongo_ext` with the C extensions for the
MongoDB Ruby driver:

    sudo gem install mongo_ext

# Neo4j

  * [Neo4j](http://neo4j.org/)  is a __graph database__. It is an embedded,
    disk-based, fully transactional Java persistence engine that stores data
    structured in graphs rather than in tables. A graph (mathematical lingo
    for a network) is a flexible data structure that allows a more agile
    and rapid style of development.

  * [Neo4j.rb](http://github.com/andreasronge/neo4j/) includes a Lucene warpper.

and

  * [Ontopia](http://code.google.com/p/ontopia/) for building, maintaining,
    and deploying Topic Maps-based applications.

# Virtuoso

  * OpenLink [Virtuoso](http://virtuoso.openlinksw.com/) Universal Server

    is a scalable cross-platform server that combines SQL/RDF/XML Data Management
    with Web Application Server and Web Services Platform functionality.

    [Open-Source Edition](http://virtuoso.openlinksw.com/dataspace/dav/wiki/Main/)

  * [OpenLink ODBC Adapter for Ruby on Rails / Active Record](http://odbc-rails.rubyforge.org/)
