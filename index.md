---
layout: default
title: PeerDrive
---

PeerDrive is a open source file system to securely store, organize, share and
sync your files from everywhere. It is built on a purely distributed
peer-to-peer data model and will be a perfect solution when you need your data
on different devices in different locations without relying on a permanent
network connection or central infrastructure.

Currently PeerDrive is in the alpha stage and hence (unless you're really
brave) not ready for productive use. The basic design is settled and there is a
prototype implementation of the file system in Erlang. Mounting via FUSE/Dokan,
network transparency and automatic synchronization/replication are roughly
working.  Additionally some small GUI applications exist to demonstrate the
full feature set.

The features
============

Store
-----

PeerDrive is mountable as a regular file system through FUSE and Dokan, thus
supporting all major operating systems. All objects in PeerDrive are versioned
so you never have to worry overwriting or loosing important data again. If the
application is PeerDrive aware you even have to never save your work
explicitly. A new version is created when you close a document or whenever you
like.

Sync
----

All PeerDrive volumes can be synchronized directly, either locally or through
the network. No central server or infrastructure is needed. The synchronization
will just update documents which are shared between the volumes and that have
been changed since the last synchronization. All types of conflicts are handled
and no data will be lost because the objects history is always kept.

Backup
------

Backups are integrated seemlessly in PeerDrive and are just a matter of adding
a synchronization rule. All new versions are forwarded to the backup volume and
kept there forever. Optionally, very old versions can be deleted from the local
volume to free disk space. The old versions of a file are instantly available
as soon as the backup volume is mounted.

Organize
--------

PeerDrive allows you to organize your files in arbitrary, non-hierarchical
ways. The links between folders and files are location independent and work
reliably across volume boundaries. Additionally any meta data, including links
to other files, can be added to a file or folder.

Screenshots
===========

{% for post in site.categories.screenshots reversed %} [![](/screenshots/images/small/{{post.image}})]({{ post.url }}) {% endfor %}

View it in action
=================

<object style="height: 390px; width: 640px">
	<param name="movie" value="http://www.youtube.com/v/mURAXMt0rLg?version=3&feature=player_detailpage"/>
	<param name="allowFullScreen" value="true"/>
	<param name="allowScriptAccess" value="always"/>
	<embed src="http://www.youtube.com/v/mURAXMt0rLg?version=3&feature=player_detailpage" type="application/x-shockwave-flash" allowfullscreen="true" allowScriptAccess="always" width="640" height="360"/>
</object>

<p></p>
