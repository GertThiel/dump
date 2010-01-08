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

# MongoDB

[Why I think Mongo is to Databases what Rails was to Frameworks](http://railstips.org/2009/12/18/why-i-think-mongo-is-to-databases-what-rails-was-to-frameworks)

  * [MongoDB](http://www.mongodb.org/)

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
