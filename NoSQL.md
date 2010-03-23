# NoSQL

  * [NoSQL](http://nosql-databases.org/)

## Alfresco ECMS

  * [Alfresco](http://www.alfresco.com/),
    [Planet](http://blogs.alfresco.com/planet/),
    [Webcasts](http://blogs.alfresco.com/wp/webcasts/)

  * Alternative front ends

    * [DoCASU](http://docasu.sourceforge.net/) uses [Ext JS](http://www.extjs.com/) 2.0

    * [Jibe](http://jibeframework.org/) uses [Ext JS](http://www.extjs.com/)

    * [opsoro](http://www.opsoro.org/) uses [Ext JS](http://www.extjs.com/) 2.0

  * Integrations

    * [Drupal](http://drupal.org/) [CMIS Alfresco Module](http://drupal.org/project/cmis_alfresco),
      [screencast](http://ecmarchitect.com/archives/2009/04/07/955)

    * [Kofax](http://www.kofax.com/de/) [Release Script](http://wiki.alfresco.com/wiki/Kofax_Release_Script)

    * Rails [CMIS Framework](http://code.google.com/p/railscmis/)

  * Misc

    * Jeff Potts [ecmarchitect.com](http://ecmarchitect.com/) site

    * [Sustainable IDE](http://www.side-labs.org/),
      based on [TOPCASED](http://www.topcased.org/),
      based on [Eclipse EMF](http://www.eclipse.org/modeling/)

## GT.M, M/DB, M/DB:X

  * [GT.M](http://fis-gtm.com) Database Engine with Extreme Scalability and Robustness

    [Documentation](http://fisglobal.com/Products/TechnologyPlatforms/GTM/UserDocumentation/index.htm)

  * [M/DB](http://gradvs1.mgateway.com/main/?path=mdb)
    is a Free Open Source "plug-compatible" alternative to
    Amazon's [SimpleDB](http://aws.amazon.com/simpledb/) database

  * [M/DB:X](http://gradvs1.mgateway.com/main/?path=mdbx)
    is a simple, lightweight, yet powerful hybrid JSON/Native XML Database

  * [M/Wire](http://gradvs1.mgateway.com/main/?path=mwire)

  * Enterprise Web Developer ([EWD](http://gradvs1.mgateway.com/main/?path=ewd))
    is an advanced web application delvelopment technology and Ajax framework

  * [PIP](http://sourceforge.net/projects/pip/) includes a JDBC driver and a
    SQL engine

    This [forum thread](http://sourceforge.net/projects/pip/forums/forum/63826/topic/1955387)
    includes hints how to integrate PIP into an existing GT.M installation

  * [Using SimpleDB and Rails in No Time with ActiveResource](http://developer.amazonwebservices.com/connect/entry.jspa?externalID=1242)

  * [gtm-rb](http://github.com/aemadrid/gtm-rb) is a first draft of a Ruby
    client library for the GT.M database engine through the M/Wire protocol

### Caché

  * InterSystems [Caché](http://www.intersystems.de/cache/) is an advanced
    but commercial 'successor' of GT.M

    Data stored in Caché can be accessed using JDBC and ODBC.

  * Max Lapshin wrote a related [Ruby driver](http://intersys.rubyforge.org/)

## Lucene + Solr

> Although Lucene is a search index, and not a database, if your fields are
> reasonably small, you can ask Lucene to store them in the index.

  * Apache [Lucene](http://lucene.apache.org/) full-text search index

  * Apache [Solr](http://lucene.apache.org/solr/) enterprise search platform

  * [Lucene or a Database? Yes!](http://lingpipe-blog.com/2008/11/22/lucene-or-a-database-yes/)

  * [Using Lucene like a relational database](http://stackoverflow.com/questions/828714/using-lucene-like-a-relational-database)

Ruby on Rails integrations:

  * [ActiveLucene](http://github.com/dcrec1/active_lucene) is like
    ActiveRecord but with Lucene the full text search engine.

    [Full text search in JRuby with ActiveLucene](http://www.diegocarrion.com/2010/02/04/full-text-search-in-jruby-with-activelucene/)

  * [ActsAsSolrReloaded](http://github.com/dcrec1/acts_as_solr_reloaded)

    [ThinkingSphinx exits, enters ActsAsSolrReloaded](http://www.diegocarrion.com/2010/01/18/thinkingsphinx-exits-enters-actsassolrreloaded/)

  * [Sunspot](http://github.com/outoftime/sunspot) Solr-powered search for
    Ruby objects

## MongoDB

> [Notes on MongoDB](http://www.paperplanes.de/2010/2/25/notes_on_mongodb.html),
> [Why I think Mongo is to Databases what Rails was to Frameworks](http://railstips.org/2009/12/18/why-i-think-mongo-is-to-databases-what-rails-was-to-frameworks),
> [MySQL and MongoDB working together in Kanbanery](http://lunarlogicpolska.com/blog/2010/02/15/mysql-and-mongodb-working-together-in-kanbanery)
> thanks to the awesomeness of [DataMapper](http://datamapper.org/)

  * [MongoDB](http://www.mongodb.org/)

  * [DataMapper MongoDB Adapter](http://github.com/solnic/dm-mongo-adapter)

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

more resources

  * [MongoHub](http://github.com/bububa/MongoHub) is a MongoDB GUI tool
    based on Titanium

  * [MongoTips](http://mongotips.com/)

### Install MongoDB

#### Mac OS X

    port install mongodb

#### Ubuntu

### Install mango\_mapper

Install `mongo_mapper` which will install the MongoDB Ruby driver `mongo`
and `jnunemaker-validatable` as well:

    sudo gem install mongo_mapper

Optionally install `mongo_ext` with the C extensions for the
MongoDB Ruby driver:

    sudo gem install mongo_ext

## Neo4j

  * [Neo4j](http://neo4j.org/)  is a __graph database__. It is an embedded,
    disk-based, fully transactional Java persistence engine that stores data
    structured in graphs rather than in tables. A graph (mathematical lingo
    for a network) is a flexible data structure that allows a more agile
    and rapid style of development.

  * [Neo4j.rb](http://github.com/andreasronge/neo4j/) includes a Lucene wrapper.

and

  * [InfoGrid](http://infogrid.org/) is an Internet __Graph Database__ with
    many additional software components that make the development of REST-ful
    web applications on a graph foundation easy.

  * [Ontopia](http://code.google.com/p/ontopia/) for building, maintaining,
    and deploying Topic Maps-based applications.

### Use Cases

  * [Access Control Lists with Graph Databases](http://nosql.mypopescu.com/post/420668099/access-control-lists-with-graph-databases)

## Persevere

  * [Persevere](http://www.persvr.org/)

## Virtuoso

  * OpenLink [Virtuoso](http://virtuoso.openlinksw.com/) Universal Server

    is a scalable cross-platform server that combines SQL/RDF/XML Data Management
    with Web Application Server and Web Services Platform functionality.

    [Open-Source Edition](http://virtuoso.openlinksw.com/dataspace/dav/wiki/Main/)

  * [OpenLink ODBC Adapter for Ruby on Rails / Active Record](http://odbc-rails.rubyforge.org/)
