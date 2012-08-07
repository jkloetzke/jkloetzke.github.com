---
layout: post
title: Announcing first release of PeerDrive
section: blog
---

I'm happy to announce the [first release of PeerDrive
(0.1.0)](https://github.com/jkloetzke/peerdrive/zipball/0.1.0).  This is a
major milestone of the project which has been cooking silently since the last
three years in my spare time.

Current status
--------------

So for what it is useful at the moment? Well, you can already use it as regular
file system to store your files. PeerDrive will automatically keep the history
of all files and folders and you can easily sync them, either locally or
through the network. Think of it as a *git*-like file system without the
restriction to synchronize the whole tree but only the parts that you want.

But more importantly, it lays the foundation of a coherent filing system that
goes far beyond the limited hierarchical file systems that we all use today.
PeerDrive brings the building blocks to enable non-hierarchical organization of
your data, reliable, extensible meta data and distributed access,
synchronization and versioning. As such it is capable of providing an
integrated solution to otherwise isolated, domain specific services/protocols
(e.g. DropBox, TimeMachine, SyncML, \*DAV) and to bring file management back on
par with todays user expectations.

Call for contributors
---------------------

Help would be very much appreciated! Basically the current state is just the
beginning of a probably very long journey. PeerDrive will make most sense with
native applications that unleash the full potentials. The current server and
client applications desperately need improvements, bug fixes, documentation,
translation, you name it. Other implementations of the PeerDrive file system
model are also highly encouraged. After all PeerDrive's strength should be to
build an open ecosystem as opposed to walled gardens like DropBox, SkyDrive et
al.

Disclaimer
----------

As the version number 0.1.0 suggests this release is far from
being stable. You may experience data loss, especially if the PeerDrive server
is not shut down properly, there is no fsck utility yet and APIs may change in
backwards incompatible ways. Still, PeerDrive is already usable and provides an
exciting potential, IMHO.

