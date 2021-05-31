# Version Control Summary.

Version Control is a system that allows you to upload your own projects, share them and record any change that occurs to your projects along side allowing you to revisit any previous
versions of your projects.

###### Centralized Version Control

It all started by programmers making their owr VCS stored on their harddrives, but need for collaboration within a developer team on a single file or set of files led to the advent of the Centralized Version Control System (CVCS). 
This system entails a single server storing all changes and file versions, which can be accessed by various clients. This streamlined the collaboration process (by eliminating the need to involve all local databases).
, but this system has __the major vulnerability of the CVS: the server as a single point of failure. If a CVS goes down, collaborators cannot work with each other on a file or save changes and new versions__.

###### Distributed Version Control

Distributed Version Control systems (DVCS) addresses the major vulnerability of the CVS *which is mentioned above* by allows clients to create mirrored repositories. These data backups can be easily be placed on the server to replace any lost information.

###### Git

Git is a DVCS(Distributed Version Control systems) that stores data in a file system made up of snapshots. Each time you save a changed version of your project **called commit** Git creates a snapshot or in simpler words, a copy of the file and stores a reference to it, it also tracks your changes and prevents data loss.
