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

Since RackDAV does not support access control we need to evaluate implementing
Stanza's WebDAV service using [Apache Jackrabbit](http://jackrabbit.apache.org/),
a Content Repository for Java (JCR) implementation, and JRuby.

## Alternatives

  * CIFS

  * JCR

## Hierarchy of Resources

    root
      projects
        imports
        tasks
        user assignments
      tasks
        complements
      users
        project assignments
