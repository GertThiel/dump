# Stanza with a WebDAV-powered frontend

The two most common means to manage unstructured data are files on a
filesystem and the hypertext of the World Wide Web.

If Stanza could publish its data as folders and files on a virtual drive,
users could manage their data with well known tools like the Finder or the
Windows Explorer.

Both [FUSE: Filesystem in Userspace](http://fuse.sourceforge.net/) and
[WebDAV](http://www.webdav.org/) are viable methods for this challenge.

## FUSE

[FuseFS](https://rubyforge.org/projects/fusefs/) is the Ruby binding for the
[FUSE](http://fuse.sourceforge.net/) library. There is also a
[repository](http://github.com/rzownir/fusefs) of FuseFS at Github.

There is [RFUSE](http://rubyforge.org/projects/rfuse/) as well which seem to
be abandoned by its author a long time ago.

[MacFUSE](http://code.google.com/p/macfuse/) is a port of FUSE to Mac OS X.

## WebDAV

Using [RackDAV](http://github.com/georgi/rack_dav) Stanza could be augmented
with a WebDAV service.

## JCR

Since RackDAV does not support access control we need to evaluate implementing
Stanza's WebDAV service using [Apache Jackrabbit](http://jackrabbit.apache.org/),
a Content Repository for Java (JCR) implementation, and JRuby.

Shen Liu of ThoughtWorks, Beijing, published a
[Rails + JCR Sample](http://github.com/wpc/jcr-rails-demo) using JRuby and
Apache Jackrabbit.

## CIFS

[Alfresco JLAN Server](http://www.alfresco.com/products/aifs/) is an
embedded virtual file system which looks just like a shared drive to the
end user. This is accomplished transparently to the user with zero client on
the desktop. JLAN supports the __CIFS__, __FTP__ and __NFS__ protocols.

## IMAP

Alfresco [supports](http://wiki.alfresco.com/wiki/Alfresco_Labs_3.2_Preview2_IMAP)
the __IMAP__ and SMTP protocols since Alfresco Labs 3.2 Preview2.

## CalDAV

[Bedework](http://www.bedework.org/): Open Source Calendar System for the
Enterprise; includes a [CalDAV](http://en.wikipedia.org/wiki/CalDAV) server;
written in Java.

## Misc

  * [MAPI](http://en.wikipedia.org/wiki/Messaging_Application_Programming_Interface):
    JuMAPI,
    [OpenMAPI](http://openmapi.org/), [OpenChange](http://www.openchange.org/)

    Regarding JMAPI and JuMAPI:  
    "Because jmapi, the java version of OpenMapi is not ready yet, we're using
    JuMAPI, the Java MAPI for teamXchange from VIPcom for now. JuMAPI is also
    part of conversations, the open source edition of teamXchange, which is
    licensed under the AGPL. It can also be used to connect to the OpenMAPI-Proxy."
    — [Source](http://osbl.wilken.de/wiki/index.php/Con:nect)

  * [TAPI](http://en.wikipedia.org/wiki/Telephony_Application_Programming_Interface)

## Hierarchy of Resources

Objects

  * documents/files ... contracts, emails
    * access control lists
  * projects ... textprovider, tts
    * imports
    * items/__tasks__/tickets
    * assignments -> user
  * appointment/events/items/tasks
    * complements
  * users
    * assignments -> project

Facets

  * by category, context, file
  * by folder
  * by project
  * by tag (cloud)
  * by user
