# Collective IQ

## What the heck is this about?

  * Track all interactions with companies and people

    * Log calls, documents, emails --> Unified messaging

    * Remind of later activities

    * Identify 'value of customers' and trouble makers

  * Manage projects

    * Compare planned and actual costs

    * Track expenses and incomes

    * Manage textprovider.de projects

      Stanza Integration…

  * Ensure compliance + Supervise all responsibilities

    Contracts: duties & rights, due dates

  * Keep all documents and records

    Scan, OCR and archive incoming paper documents and snail mails

## Domains and Features

  * Contacts and Relations Management (CRM) + Groupware (Gw)

    * Activities, Calendar, Events …

      Call log, TAPI integration

    * Contracts + Compliance

    * E-Mails

  * Documents + Files (DMS)

    * Scan, OCR and import snail mails

      Integrate a native Mac or Windows scanning software: Kofax…

  * Project Management (PM)

    * Trouble Tickets (TTS)

    * Software Change Management (SCM) Integration

  * Stanza Integration

    * Tasks

  * Content Management System (CMS)

    * Customer Websites

    * Documentation

## Optional Domains and Features

  * Crawling Proxy

    Let users browse using an integrated HTTP proxy to index all visited
    web sites for later retrieval

## CIQ Modules

### CIQ: Assistant

  * Customer and Contacts Mgmt. (CRM)

  * Personal Information Mgmt. (PIM)

  * Unified Messaging (UM)

optionally

  * Business Intelligence (BIS)

  * Instant Messaging (IM)

  * Crawlers and indexing Bots and Proxies

  * Synchronization with PDAs and smart phones

__textprovider.de__ related project aquisition belongs here

### CIQ: Project

— Projektsteuerung / -verwaltung

  * Project Mgmt. (PM) including Resource Planning (ERP, HRIS)

  * Defect and Requirement Mgmt. (TTS)

  * Software Change Mgmt. (SCM)

__Stanza__ software development belongs here

### CIQ: Stanza

  * Content Mgmt. (CMS)

    integrates __textprovider.de__ by delegating content authorships as tasks.

    Shall replace the SilverStripe installation for the textprovider.de site.

  * textprovider.de (TP)

    offers SEO-compliant content production.

optionally

  * Linguistics

    integrates dictionaries, thessauri, text corpora… like:
    dict.cc, Duden, Google, leo.org, Pons, Wikipedia, Wiktionary, Wordnet, Yahoo

  * Remote content mgmt.

    Tightly integrate external and remote content management systems like
    Drupal, Joomla or Wordpress. Sell remote authoring as a service
                                           — Fernredaktion als Dienstleitung.

__textprovider.de__ related task settlements belong here

### CIQ: Vault

  * Document Lifecycle Mgmt. (DMS)

    including

    * contract and compliance mgmt.

    * scanning and indexing of paper documents

      by integrating an external native Mac OS X or Windows application like
      Kofax

    * software source repositories
    
    * and any other persisted information that's value does not depend on
      ownership or time

  * Indexing of external and remote repositories

__textprovider.de__ related outcomes (exports) belong here

## Minimum Record Types

Information vs. Context -- Information ./. Zusammenhang

Links declare contexts -- Verknüpfungen bilden Zusammenhänge ab

  * CONTACT -- KONTAKT

    <-- File / Item

    --> Company, contact person, user -> author, reviewer, manager…

    A contact represents a person; be it a company or a human being.

    Contacts may include contacts: A company — Firma — record usually includes
    at least one contact person — Ansprechpartner.

    May be tagged to be an author or reviewer, a customer, a partner

        Contact
          -> Contact persons, each a contact of it's own
          -> Addresses

  * Address

    <-- File / Item

    --> Email address, postal address

    Some kind of __location__.

  * Activity -- Tätigkeit

    <-- Event + linked Contacts with roles

    --> Appointment, task

    Activities are events which some one attends to or manages. It's not about
    the event but about someone doing something regarding an event as her/his
    role requires.

    Every texprovider.de task is an activity. Author, reviewer and project
    manager are respnsible for the successful settlement of a task.

    Activities can be composed of many: Visiting a customer depends on
    travelling there and back:
                                                   — Anreise, Termin, Abreise

        Activity
          -> Contacts + Roles
          -> Event

  * EVENT -- EREIGNIS

    <-- File / Item

    Events happen at or from and until some __time__s.

    Birthdays, holidays …

        Event
          Range: Start date and end date (optionally with time)
          Recurrences (optionally)

  * File / Item -- Akte

    May be a document, an email or any record

    Files implicitly define a context across all subsidiary items.

## Inspirations

  * [Chandler](http://chandlerproject.org/)

  * Corel InfoCentral

  * [Ecco Pro](http://en.wikipedia.org/wiki/Ecco_Pro)

  * [InfoCube](http://www.infoqube.biz/)

  * Lotus [Agenda](http://en.wikipedia.org/wiki/Lotus_Agenda),
    [Organizer](http://en.wikipedia.org/wiki/Lotus_Organizer)

and

  * [DabbleDB](http://dabbledb.com/)
