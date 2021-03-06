# TorqueBox

  * should implement often required Rails app features using JBoss AS services

    and offer drop-in replacements of popular Rails extensions like
    restful-authentication, Delayed::Job

  * should expose popular JBoss AS and other libraries features to Rails apps

    and allow developers to update their Rails applications with advanced
    features like instant cloud-readyness, enterprise-grade integration or
    service management and monitoring easily

  * should behave exactly like plain Rails deployments until the user
    configures the app to take adavantage of TorqueBox features

    ActionController::Base.cache\_store = :jboss\_cache\_store

> If I have seen further it is only by standing on the shoulders of giants.


## Caveat Lector

__All code snippets show proposals only!__ In fact the complete document is a
collection of ideas and proposals.


## Features

TorqueBox should implement or integrate features on-the-fly and in an
unobtrusive manner wherever possible.

Features that depend on JBoss AS should be configured with or inherited from
sources located in separate directories which could be easily excluded if the
Rails app or part of it needs to be deployed traditionally, that is without
JBoss AS.

E.g. `app/dav_presenter`…


### Session Store

TorqueBox should provide a clustered session store and use that if
configured to do so:

    ## in config/initializers/session_store.rb

    ActionController::Base.session_store = :jboss_session_store

Caveat utilitor: Replacing a default Rails session store with the JBoss
session store invalidates every existing session (cookie)!


### Cache Store

TorqueBox should provide a clustered cache store and use that if
configured to do so:

    ## in config/initializers/cache_store.rb

    ActionController::Base.cache_store = :jboss_cache_store
    ActionController::Base.cache_store = :infinispan_store
    ActionController::Base.cache_store = :compressed_jboss_cache_store
    ActionController::Base.cache_store = :compressed_infinispan_store

Integrate ActiveSupport::Cache with [JBoss Cache](http://jboss.org/jbosscache/)
and [Infinispan](http://www.jboss.org/infinispan/)

Specifications: JCACHE

Status: Beta, available


### Embedded Database

TorqueBox should provide a clustered and embedded database suitable to replace
SQLite and use that if configured to do so:

    ## in config/database.yml

    test:
      adapter: hypersonic

While most deployments will continue to use MySQL, PostgreSQL or another
dedicated RDBMS server such an embedded database could be useful for testing
proposes.


### Authentication and Authorization

TorqueBox should …

Specifications: JAAS, OpenId, OAuth

[restful-authentication](http://github.com/technoweenie/restful-authentication),
[authlogic](http://github.com/binarylogic/authlogic/),
[clearance](http://github.com/thoughtbot/clearance/)

[JBoss Security](http://jboss.org/jbosssecurity/),
[JBossXACML](http://jboss.org/jbosssecurity/jbossxacml.html)
and desktop and web app single sign-on with
[JBoss Negotiation](http://jboss.org/jbosssecurity/jbossnegotiation.html)


### Identity

TorqueBox should …

[JBoss Identity](http://www.jboss.org/jbossidentity/)


### Misc Security

TorqueBox should …

Specifications: OAuth


### Server and Service Management and Monitoring

TorqueBox should …

Specifications: JMX

[Jopr](http://jboss.org/jopr)


### State Machines and Workflows

TorqueBox should integrate … a worklow engine … orchestrate a Rails app …

Specifications: BPEL, XPDL

[Ruote](http://openwferu.rubyforge.org/) formerly known as OpenWFEru

[Drools Guvnor](http://jboss.org/drools/drools-guvnor.html),
[Drools Flow](http://jboss.org/drools/drools-flow.html),
[JBoss jBPM](http://jboss.org/jbossjbpm/),
[JBoss BPEL Server](http://jboss.org/riftsaw) aka RiftSaw,
[POC-UI](http://www.pocui.org/)

    # in app/flows/…


### Database Access and Full Text Search

TorqueBox should integrate ActiveRecord behind the scenes with JDBC.

TorqueBox should integrate ActiveRecord behind the scenes with Hibernate and
make advanced features like __Hibernate Search__ available to the Rails app.
Such an integration could render external full text search engines like Ferret
or Sphinx and the Rails plug-ins superfluous.

Specifications: JDBC

ActiveRecord, Datamapper, Ferret, Sphinx

[Hibernate](https://www.hibernate.org/)

Banks: [ActiveHibernate](http://code.google.com/p/activehibernate/),
ActiveJPA: allow all Java Persistence frameworks to be swapped under the covers

Status: Released, packaged w/ TorqueBox


### Content Repositories

TorqueBox should …

Specifications: JCR

[JBoss DNA](http://jboss.org/dna/)


### Markdown and Textile

<del>[Radeox Wiki Render Engine](http://codemonkeyism.com/forking-radeox-a-new-wiki-render-engine/)</del>,
<del>[Wiki Model](http://wikimodel.sourceforge.net/)</del>,
[XWiki Rendering Module](http://code.xwiki.org/xwiki/bin/view/Modules/RenderingModule)

    # in app/models/document.rb

    class Document < ActiveRecord::Base

      markup :content

    end

    document = Document.find(:first)

    document.content = " … ".markup(:from_html4)
    document.content = " … ".markup(:from_markdown)
    document.content = " … ".markup(:from_textile)
    document.content = " … ".markup(:from_xhtml)

    document.content.to_html4
    document.content.to_markdown
    document.content.to_textile
    document.content.to_xhtml


### Integration: WebDAV

TorqueBox should allow to expose 'stuff' to WebDAV clients using a presenter.

    # in app/dav_presenters/document_dav_presenter.rb

    class DocumentDavPresenter < TorqueBox::DavPresenter

      # expose the default controller actions (index, show, update, delete…)
      #
      # caveat utilitor: creating instances of Document can be an issue
      #
      expose :Document

      # expose the default controller actions (index, show, update, delete…)
      # and include 'fake' documents which will be generated by calling
      # a non-default action and streamed to the WebDAV-client on-the-fly
      # when this file is loaded
      #
      expose :Document do
        prepare :generate_summary, :cache_for => 1.day
      end

    end


### Integration: ESB, REST, SOA, SOAP, Webservices

TorqueBox should …

Specifications: SOAP, WS-*

[ActionWebService](http://github.com/datanoise/actionwebservice)

[JBossESB](http://jboss.org/jbossesb/),
[JBossWS](http://jboss.org/jbossws/)

Bank: [handsoap](http://github.com/troelskn/handsoap)

    class Ec2Endpoint << TorqueBox::Soap::Endpoint

      # configure the defaults of this class
      #
      service 'AmazonEC2' do
        description 'public/system/wsdl/ec2.wsdl'
        namespace   'http://ec2.amazonaws.com/doc/2008-12-01/'
      end

      # overwrite everything that should be handled
      # individually

      # method per operation

    end

    # or

    class Ec2Endpoint

      include TorqueBox::Soap::Endpoint

      # method per operation

    end

Status: Beta, partitially packaged w/ TorqueBox


### Integration: Messaging

TorqueBox should …

Specifications: JMS

[HornetQ](http://jboss.org/hornetq/)


### Integration: Thrift

[Thrift](http://incubator.apache.org/thrift/),
[thrift4rails](http://github.com/railsbros/thrift4rails)

    # in app/endpoints/document_thrift_endpoint.rb

    class DocumentThriftEndpoint << TorqueBox::Thrift::Endpoint

      # method per operation

    end

    # or

    class DocumentThriftEndpoint

      include TorqueBox::Thrift::Endpoint

      # method per operation

    end


### Data Warehousing and Mining

TorqueBox should …

[ActiveWarehouse](http://github.com/aeden/activewarehouse)

[Teiid](http://www.jboss.org/teiid/)


### Portals and Portlets

Specifications: Portlets 2.0


### Misc

TorqueBox should allow to expose 'stuff' as Excel- and PDF/RTF download as
part of scaffolded ActionControllers by leveraging
[Apache POI](http://poi.apache.org/) and [iText](http://www.lowagie.com/iText/).

TorqueBox should spell check 'stuff' using
[Hunspell](http://hunspell.sourceforge.net/) and
[ruby-hunspell](http://rubyforge.org/projects/ruby-hunspell/) or
[hunspell](http://rubyforge.org/projects/hunspell)

### Licensing

TorqueBox should only depend on and include features, libraries and other
stuff that's available under commercial use-friendly licenses like APL, LGPL
or MIT-license.
