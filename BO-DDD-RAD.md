# BO, DDD, RAD

## CQRS, ES

Edument's [CQRS Starter Kit](http://cqrs.nu/)

Jacek Laskowski's [Rough Notes about CQRS and ES](https://gist.github.com/jaceklaskowski/d267bf4176822293e95e) has many related links

[Stream processing, Event Sourcing, Reactive, CEP … and making sense of it all](http://www.confluent.io/blog/making-sense-of-stream-processing/)

### Elixir, Erlang

 * Bryan Hunter's [Elixir CQRS Eventstore](https://github.com/bryanhunter/elixir_cqrs_es) is a port of his [CQRS with Erlang](https://github.com/bryanhunter/cqrs-with-erlang/tree/ndc-oslo)

### Java

 * [Axon Framework](http://www.axonframework.org/)

   [Grails + Axon Framework = CQRS](http://blog.dblazejewski.com/2013/11/grails-axon-cqrs-part-i.html), [part 2](http://blog.dblazejewski.com/2013/11/grails-axon-cqrs-part-ii.html)

### Ruby

[Fast introduction to Event Sourcing for Ruby programmers](http://blog.arkency.com/2015/03/fast-introduction-to-event-sourcing-for-ruby-programmers/), [Why use Event Sourcing](http://blog.arkency.com/2015/03/why-use-event-sourcing/)

[From ActiveRecord to Event Sourcing](http://de.slideshare.net/emadb/wroclove-rb) by Emanuele DelBono

[Introduction to CQRS / ES with Rails](http://praglowski.com/presentations/cqrses/drug/) by Mirosław Pragłowski, his [example](https://github.com/mpraglowski/cqrses-sample/) depends on Greg's Event Store

#### Libraries

 * Greg's [Event Store](https://geteventstore.com/), the open-source, functional database with Complex Event Processing in JavaScript

   [Explaining Greg's Event Store](http://blog.arkency.com/2015/03/explaining-gregs-event-store/), [Your solid tool for event sourcing - EventStore examples](http://blog.arkency.com/2015/03/your-solid-tool-for-event-sourcing-eventstore-examples/) [Stream pagination in Greg's Event Store](http://blog.arkency.com/2015/03/stream-pagination-in-gregs-event-store/), all by Tomasz Rybczyński, leading to …

   Arkency's [HttpEventstore](https://github.com/arkency/http_eventstore) is a Ruby HTTP connector to Greg's Event Store

   [How to use Greg's Event Store from Ruby](http://blog.arkency.com/2015/03/how-to-use-gregs-event-store-from-ruby/) by Tomasz Rybczyński, leading to …

 * [Arkency](http://blog.arkency.com/)'s [RubyEventStore](https://github.com/arkency/ruby_event_store) is a Ruby implementation of an Event Store and an integral part of the Arkency's [RailsEventStore](https://github.com/arkency/rails_event_store) based on Active Record

   [The Event Store for Rails developers](http://blog.arkency.com/2015/04/the-event-store-for-rails-developers/) by Tomasz Rybczyński

   [Building an Event Sourced application using RailsEventStore](http://blog.arkency.com/2015/05/building-an-event-sourced-application-using-rails-event-store/), [Using domain events as success/failure messages](http://blog.arkency.com/2015/05/using-domain-events-as-success-slash-failure-messages/), all by Mirosław Pragłowski

   [Introducing Read Models in your legacy application](http://blog.arkency.com/2015/05/introducing-read-models-in-your-legacy-application/) by Rafał Łasocha

 * [Rails Disco](https://github.com/hicknhack-software/rails-disco) — a distributed party with commands, events and projections, [Examples](https://github.com/hicknhack-software/rails-disco-examples)

   [Rails Disco: Get Down with Event Sourcing](http://www.sitepoint.com/rails-disco-get-event-sourcing/)

 * Ruby CQRS aka [rcqrs](https://github.com/slashdotdash/rcqrs) and [rcqrs-rails](https://github.com/slashdotdash/rcqrs-rails) with Event Sourcing

[Event Sourcing Libraries in Ruby: A Guide](http://fhwang.net/g/Event-Sourcing-Libraries-in-Ruby-A-Guide) presents besides `RailsEventStore` …

 * [Event Sourced Record](https://github.com/fhwang/event_sourced_record) offers an idiomatic way to use the Event Sourcing pattern in Rails code

 * [Sandthorn Event Sourcing](https://github.com/Sandthorn/sandthorn) is a Ruby library for saving an object's state as a series of events, depends on Sequel

#### Without libraries

 * [The CQRS diet](http://de.slideshare.net/cavalle/the-cqrs-diet) by Luismi Cavallé and it's example [BankSimplistic](https://github.com/cavalle/banksimplistic)

 * [Event sourcing on Rails with RabbitMQ](http://codetunes.com/2014/event-sourcing-on-rails-with-rabbitmq/) by Tymon Tobolski

### Scala

 * [Scala CQRS Framework](https://stackoverflow.com/questions/8609664/scala-cqrs-framework) on Stack Overflow mentions [Akka Persistance](http://doc.akka.io/docs/akka/2.4.0/scala/persistence.html) and it's inspiration [eventsourced](https://github.com/eligosource/eventsourced)

   Martin Krasser, the author of both `eventsourced` and `Akka Persistance`, wrote a blog to compare the latter with [Eventuate](https://rbmhtechnology.github.io/eventuate/) which he wrote as well

 * [CQRS/ES in Scala: an overview](http://www.hyperlambda.com/posts/cqrs-es-in-scala/) lists three CQRS/ES examples in Scala:

   * [CQRS with Akka actors and functional domain models](http://debasishg.blogspot.co.uk/2011/01/cqrs-with-akka-actors-and-functional.html),

   * [Akka DDDD template using CQRS/ES with a Distributed Domain](https://github.com/boldradius/akka-dddd-template#master) and

   * Paweł Kaczor's [ddd-leaven-akka-v2](https://github.com/pawelkaczor/ddd-leaven-akka-v2)

## Hexagonal Architecture

 * [A place to discuss and experiment with Hexagonal Architecture in Ruby and Rails](https://github.com/padwasabimasala/hexagonal-ruby)


## Naked Objects

 * [Apache Isis](https://isis.apache.org/), formerly Naked Objects, [Add-ons](http://www.isisaddons.org/), [Dan Haywood's Blog](http://danhaywood.com/)

 * [JMatter](http://jmatter.org/) is a software framework for constructing workgroup business applications based on the [Naked Objects Architectural Pattern](https://en.wikipedia.org/wiki/Naked_objects)

 * [Naked Objects.NET](http://nakedobjects.codeplex.com/) ([GitHub](https://github.com/NakedObjectsGroup/NakedObjectsFramework))


## Micro Services

 * [fabric³](http://www.fabric3.org/)

 * [fabric8](http://fabric8.io/)


## Misc

 * [Eclipse Scout](http://www.eclipse.org/scout/), [Eclipse Scout Blog](http://www.bsiag.com/scout/), [BSI](http://www.bsiag.com/de/technologien/eclipse-scout.html)

 * [JVx](http://www.sibvisions.com/de/jvx)

 * [OpenXava](http://openxava.org/)

 * [Portofino](http://www.manydesigns.com/en/portofino)

 * [Roma \<Meta\> Framework](http://romaframework.org/) ([GitHub](https://github.com/romaframework))

 * [Sculptor](http://sculptorgenerator.org/) is an open source productivity tool that applies the concepts from [Domain-Driven Design](http://domaindrivendesign.org/books/) and [Domain Specific Languages](https://en.wikipedia.org/wiki/Domain-specific_language) for generating high quality Java code and configuration from a textual specification
