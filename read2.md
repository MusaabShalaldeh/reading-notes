# Version Control Summary.

Version Control is a system that allows you to upload your own projects, share them and record any change that occurs to your projects along side allowing you to revisit any previous
versions of your projects.

###### Centralized Version Control

It started by developers making their owr VCS which was stored on their harddrives,
but the need for working together in a team on a single file or a full project led for the making of Centralized Version Control System (CVCS).

This system is a single server that stores all changes and files that can be accessed by The Developers Team, this streamlined the collaboration process and made it much easier.
However, this system has the major vulnerability of being a single server, which means if this machine failed, all data stored on it is not going to be available or of it goes down, it can't be accessed by others.

###### Distributed Version Control

Distributed Version Control systems (DVCS) solves the major vulnerability of the CVS *which is mentioned above* by allowing clients to create mirrored repositories. These data backups can be easily be placed on the server to replace any lost information.

###### Git

Git is a DVCS(Distributed Version Control systems) that stores data in a file system made up of snapshots(or multiple copies of the file).

Each time a change is made, it records the change and creates a copy of the file each time a **commit** is made, so that it can be accessed later and it prevents the loss of those files.
