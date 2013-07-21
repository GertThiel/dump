# Aspect Oriented Programming

  * [Aquarium](http://aquarium.rubyforge.org/)

  * [Gazer](http://github.com/teejayvanslyke/gazer)

    [Aspect-oriented programming in Ruby with Gazer](http://www.elctech.com/projects/aspect-oriented-programming-in-ruby-with-gazer)

# Authentification, Single Sign-on and Authorization

  * [CanCan](http://github.com/ryanb/cancan)

  * [CAS](http://www.jasig.org/cas)

    * [devise_cas_authenticatable](http://github.com/nbudin/devise_cas_authenticatable)

    * [RubyCAS-Client](http://code.google.com/p/rubycas-client/) and
      [RubyCAS-Server](http://code.google.com/p/rubycas-server/)

  * [Devise](http://github.com/plataformatec/devise)

# BDD + TDD

  * [Fixtures without validation with Factory Girl](http://codetunes.com/2009/11/05/fixtures-without-validation-with-factory-girl/) -
    Nice idea for generating bad data in a concise and repeatable way

  * [Pickle](http://github.com/ianwhite/pickle) gives you Cucumber steps that
    create your models easily from FactoryGirl or Machinist factories/blueprints.

  * [Testing validity of Rails feeds with RSpec](https://wincent.com/wiki/Testing_validity_of_Rails_feeds_with_RSpec)

# Content Management Systems

  * [Rails CMS Alternatives](http://afreshcup.com/home/2009/11/26/rails-cms-alternatives.html),
    [Gist](http://gist.github.com/242751)

# Data Exchange, Import + Export

## AtomPub

### Java

  * Apache [Abdera](http://abdera.apache.org/)

  * [Atomojo](http://code.google.com/p/atomojo/)

  * [Rome Propono](http://wiki.java.net/bin/view/Javawsxml/RomePropono)

### Ruby

  * <del>[Alumina](http://github.com/inkspot/alumina) is a Ruby gem that
    implements Atom, both the syndication format and the publishing protocol</del>

  * [Atom Protocol Exerciser](http://rubyforge.org/projects/ape) is a tool
    to test your AtomPub protocol server

  * [atompub-server](http://github.com/calavera/atompub-server) to add
    AtomPub server capabilities to your Rails application

## WebDAV

Rails 2:

  * [RackDAV](http://github.com/georgi/rack_dav),
    [GridFS adapter](http://github.com/retro/gridfs-rackdav)

Rails 3:

  * [dav4rack](http://github.com/chrisroberts/dav4rack)

    [Rails 3 and DAV4Rack sample application](http://github.com/clyfe/rails3-dav4rack-example)

## Web Services

  * [Handsoap](http://rubygems.org/gems/handsoap)

  * [Savon](http://rubygems.org/gems/savon)

# Desktop Integration

  * [Add-in Express](http://www.add-in-express.com/) are sets of components,
    visual designers and wizards for developing secure, managed, isolated,
    deployable and version-neutral Microsoft Office extensions, including
    COM add-ins, Outlook plug-ins, Office smart tags, Excel RTD servers,
    Excel XLL and UDF add-ons.

# Documentation

  * [Rocco](http://rtomayko.github.com/rocco/) is a Ruby port of
    [Docco](http://jashkenas.github.com/docco/), the quick-and-dirty,
    hundred-line-long, __literate__-programming-style documentation generator

  * [YARD](http://yardoc.org/) is a documentation generation tool for the
    Ruby programming language

# Linguistics + Statistics

## Algorithmen

  * Plagiarism detection algorithms

    * Greedy String Tiling (GST),
      Running-Karp-Rabin Greedy-String-Tiling (RKS-GST)

    * nGram Overlap

    * SPEX

    * Winnowing

## Java

  * [Gate](http://gate.ac.uk/) General Architecture for Text Engineering

  * [LingPipe](http://alias-i.com/lingpipe/) is a suite of Java libraries for
    the linguistic analysis of human language

## Javascript

Strip HTML from text ([Source](http://stackoverflow.com/questions/822452/strip-html-from-text-javascript))

    jQuery(html).text();

### Libraries

  * [bjspell](https://code.google.com/p/bjspell/) JavaScript based
    spell checker compatible with Hunspell dictionaries

  * [Hyphenator.js](http://code.google.com/p/hyphenator/) Javascript that implements client-side hyphenation of HTML-Documents

  * [Hypher](http://www.bramstein.com/projects/hypher/)
    JavaScript hyphenation engine ([Github](https://github.com/bramstein/Hypher))

  * [jspos](https://code.google.com/p/jspos/) is a Javascript port of
    [Mark Watson's FastTag](http://www.markwatson.com/opensource/) part of speech tagger

  * [TextStatistics.js](https://github.com/cgiffard/TextStatistics.js)
    generates information about texts including syllable counts and
    Flesch-Kincaid, Gunning-Fog, Coleman-Liau, SMOG and Automated Readability
    scores (English only)
    (a port of [TextStatistics.php](https://github.com/DaveChild/Text-Statistics))

  * [Typo.js](http://www.chrisfinke.com/2011/03/31/announcing-typo-js-client-side-javascript-spellchecking/)
    Client-side JavaScript Spellchecking

## Ruby

  * [Completeness-Fu](http://github.com/joshk/completeness-fu)

  * [Classifier](http://classifier.rubyforge.org/) is a general module to
    allow Bayesian and other types of classifications.

  * [CRM114.rb](http://crm114.rubyforge.org/), a Ruby interface to
    [CRM114](http://crm114.sourceforge.net/) Controllable Regex Mutilator, an
    advanced and fast __text classifier__ that uses sparse binary polynomial matching
    with a Bayesian Chain Rule evaluator and a hidden Markov model to categorize
    data with up to a 99.87% accuracy.

  * [ffi-hunspell](https://github.com/postmodern/ffi-hunspell),
    Ruby FFI bindings for [Hunspell](http://hunspell.sourceforge.net)

  * Ruby [Linguistics](http://www.deveiate.org/projects/Linguistics/) Framework

  * [treetagger-ruby](https://github.com/arbox/treetagger-ruby) a Ruby based
    wrapper for the [TreeTagger](http://www.ims.uni-stuttgart.de/projekte/corplex/TreeTagger/)
    by Helmut Schmid which is the foundation of [LinguLab](http://www.lingulab.net/)

### Ruby + GNU Scientific Library

  * [GNU Scientific Library](http://www.gnu.org/software/gsl/)

  * [RubyGSL](http://rb-gsl.rubyforge.org/) is a ruby interface to the
    GSL (GNU Scientific Library), for numerical computing with Ruby.

  * [Ruby/GSL-ng](http://rubygems.org/gems/ruby-gsl-ng) is a new generation
    Ruby/GSL wrapper that strives for code simplicity while retaining
    acceptable performance. Other GSL wrappers are either utterly complicated
    (lots of C code) or poorly documented. Ruby/GSL-ng uses Ruby/__FFI__ and
    little bits of C code to achieve a simple implementation that integrates
    neatly with Ruby's standard classes and follows most of its conventions.

## Ruby + R

  * [Ruby client for Rserve](http://github.com/clbustos/Rserve-Ruby-client),
    a [binary R server](http://www.rforge.net/Rserve/)

  * [RSRuby](http://rubyforge.org/projects/rsruby/) is a port of RPy
    (the equivalent Python module) and embeds a full R interpreter into Ruby.

    Chris Lowis' [Using R and Ruby](http://blog.chrislowis.co.uk/2009/02/15/LRUG-R-Ruby-talk.html)
    slides from February 2009 LRUG demonstrate RSRuby.

    Chris Lowis [blog](http://blog.chrislowis.co.uk/) and
    [repositories](http://github.com/chrislo/) offer more statistics with Ruby
    related stuff. The [Data Visualisation with Ruby](http://github.com/chrislo/data_visualisation_ruby)
    repository demonstrates different options to __visualize data using Ruby__
    and external applications and libraries
    ([slides](http://github.com/chrislo/data_visualisation_ruby/blob/master/slides.pdf)).

  * [RRb](http://sourceforge.net/projects/rrb/) is a very simple Ruby
    interface to the R statistical computing language.

## R

[R](http://www.r-project.org/) is a free software environment for statistical
computing and graphics. [Rweb](http://www.math.montana.edu/Rweb/) is a Web
based interface to R.

  * Stefan Th. Gries'
    [Statistik für Sprachwissenschaftler](http://www.v-r.de/en/items/1001001996/), engl.
    [Statistics for Linguistics with R](http://www.degruyter.com/cont/imp/mouton/detailEn.cfm?id=IS-9783110205640-1),
    [Google Group](http://groups.google.com/group/statforling-with-r/web/statistics-for-linguists-with-r)
    mit den relevanten Dateien

  * Stefan Th. Gries'
    [Quantitative corpus linguistics with R: a practical introduction](http://www.linguistics.ucsb.edu/faculty/stgries/under_construction.html),
    [Google Group](http://groups.google.com/group/corpling-with-r/web/quantitative-corpus-linguistics-with-r)
    mit den relevanten Dateien

Stefan Th. Gries' [web page](http://www.linguistics.ucsb.edu/faculty/stgries/index.html) has more links.

## Misc

  * [Copyfind](http://plagiarism.phys.virginia.edu/)

  * [METER (MEasuring TExt Reuse) Project](http://www.dcs.shef.ac.uk/nlp/meter/)
    incl. algorithm implementations written in Perl

  * [Snowball](http://snowball.tartarus.org/) is a language in which __stemming__
    algorithms can be easily represented. The Snowball compiler translates a
    Snowball script (a  .sbl file) into either a thread-safe ANSI C program or a
    Java program.

# Linked Data + Semantic Web

  * [Linked Data](http://linkeddata.org/) is about using the Web to connect
    related data that wasn't previously linked, or using the Web to lower
    the barriers to linking data currently linked using other methods

# Markups

  * [Radius](http://radius.rubyforge.org/) is a powerful tag-based template
    language for Ruby inspired by the template languages used in
    [MovableType](http://www.movabletype.org/) and
    [TextPattern](http://textpattern.com/). It uses tags similar to XML,
    but can be used to generate any form of plain text (HTML, e-mail, etc…).

# Markdown

  * [Babelmark](http://babelmark.bobtfish.net/) Markdown Testbed

  * [MultiMarkdown](http://fletcherpenney.net/multimarkdown/)

    A derivative of the original Markdown.pl with added features by
    Fletcher T. Penney.

## Ruby

  * [kramdown](http://rubyforge.org/projects/kramdown) is
    yet-another-markdown-parser but fast, pure Ruby, using a strict
    syntax definition and supporting several common extensions

  * [Maruku](http://maruku.rubyforge.org/): a Markdown-superset interpreter

    Andrea Censi's Markdown parser with additional features, some borrowed
    from Markdown Extra.

  * [RDiscount](http://github.com/rtomayko/rdiscount)

# Project Mgmt + Team Coordination

  * [Redmine](http://www.redmine.org/)

  * [Retrospectiva](http://retrospectiva.org/),
    [GitHub repo](http://github.com/dim/retrospectiva)

  * [Teambox](http://www.teambox.com/),
    [GitHub repo](http://github.com/michokest/Teambox-2)

# Resource Description Framework (RDF)

  * [DataMapper RDF.rb Adapter](http://dm-rdf.rubyforge.org/)

  * [RDF.rb](http://rdf.rubyforge.org/): RDF API for Ruby

    [RDF.rb: A Public-Domain RDF Library for Ruby](http://blog.datagraph.org/2010/03/rdf-for-ruby)

# Telephony + VoIP

  * [Asterisk](http://www.asterisk.org/)

  * [Yate](http://yate.null.ro/) is Yet Another Telephony Engine

# Web Services

##  Mehrwertsteuernummer (MWSt-ID), Umsatzsteuernummer (USt-ID)

  * Online Formular zur
    [Bestätigung von ausländischen Umsatzsteuer-Identifikationsnummern](http://evatr.bff-online.de/eVatR/)
    des Bundeszentralamts für Steuern mit der Beschreibung einer XML-RPC
    Schnittstelle ebd.

  * [SEPA - Der einheitliche Euro-Zahlungsverkehrsraum](http://www.bundesbank.de/zahlungsverkehr/zahlungsverkehr_sepa.php)

# Web Server

  * [Hiawatha](http://hiawatha-webserver.org/)

    [HOWTO : Highest secured Hiawatha Web Server 9.0 on Ubuntu 12.04 LTS Server](http://secure-ubuntu-server.blogspot.hk/2013/03/howto-highest-secured-hiawatha-web.html)

# Misc

  * [Backup](http://github.com/meskyanichi/backup/) Databases and Files
    for Ruby on Rails and plain Unix

  * [Bluepill](http://asemanfar.com/Bluepill:-a-new-process-monitoring-tool):
    a new process monitoring tool

  * [Ernie](http://github.com/mojombo/ernie) is an Erlang/Ruby
    [BERT-RPC](http://bert-rpc.org/) Server

  * [Fail2ban](http://www.fail2ban.org/wiki/index.php/Main_Page) scans log files
    (e.g. `/var/log/apache/error_log`) and bans IPs that show the malicious signs
    — too many password failures, seeking for exploits, etc

  * [git-flow](http://github.com/nvie/gitflow) is a collection of Git extensions
    to provide high-level repository operations for Vincent Driessen's
    [branching model](http://nvie.com/git-model)

  * [httpi](http://rubygems.org/gems/httpi) provides a common interface for
    Ruby HTTP libraries: Curb, HTTPClient and Net::HTTP

  * [Liquid HTML Editor](http://github.com/tobi/liquid-editor) -
    Liquid syntax highlighting for the amazing
    [CodeMirror](http://marijn.haverbeke.nl/codemirror/) HTML source code editor

  * A more interactive Stanza frontend could be build upon
    [Node.JS](http://nodejs.org/), [Express](http://expressjs.com/),
    [Socket.IO](http://socket.io/), all three foundation of
    [Zappa](http://github.com/mauricemach/zappa),
    and [NowJS](http://nowjs.com/). See also
    [Derby](http://derbyjs.com/) ([Github](https://github.com/codeparty/derby)),
    [Meteor](http://meteor.com/) and
    [SocketStream](http://www.socketstream.org/) ([Github](http://github.com/socketstream/socketstream)).
    And [vert.x](http://vertx.io/).

    [batman.js](http://batmanjs.org/),
    [Joosy](http://joosy.ws/) ([Github](https://github.com/roundlake/joosy))

    Scala based alternatives:
    [Lift Framework](http://liftweb.net/),
    [Play Framework](http://www.playframework.org/)

  * [Piwik](http://piwik.org/) is a real time web analytics software (GPL)

  * PDF rending plug-in for Rails using
    [FlyingSaucer](https://xhtmlrenderer.dev.java.net/):
    [saucerly](http://github.com/wycats/saucerly),
    [saucerly](http://github.com/nicksieger/saucerly)

  * [RightAWS](http://rightaws.rubyforge.org/) -
    RightScale's open-source gems provide Ruby-language interfaces to several
    cloud computing platforms

  * [RSS Renderer for Rails 3](https://gist.github.com/445869/) using `ActionController.add_renderer`

  * [Ruleby](http://github.com/mattup/ruleby) - Rule Engine for Ruby

  * [Ruby on Sails](http://danopia.net/posts/12) - __Google Wave__ provider
    implemented in Ruby

  * [Semantic Versioning](http://semver.org/)

  * [Socky](http://imanel.org/projects/socky) is a complete solution for
    realtime browser-server communication using WebSockets (where available,
    falling back to flash sockets where not)

  * [Sprockets 2](http://getsprockets.org/)

    [Using Sprockets 2 in Rails 3.0.x with CoffeeScript and SASS](https://gist.github.com/911003)

    Some of [Using CoffeeScript in Rails](http://rubysource.com/using-coffeescript-in-rails/)
    is maybe useful as well

  * [Custom SQL queries without find\_by\_sql](http://snippets.dzone.com/posts/show/5570)

  * [Supermodel](http://github.com/maccman/supermodel): Simple ActiveModel-Powered In-Memory Models
