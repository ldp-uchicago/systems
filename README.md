# Legacy Systems

The LDP once had a database and sys admin named Ben (2007-2015).  He originally setup and maintained a number of machines for the LDP, SILC, and Goldin-Meadow Lab.

The [Research Computing Center](https://github.com/rcc-uchicago) now provides file system storage and other services for the LDP (See [`rcc-uchicago/ldp`](https://github.com/rcc-uchicago/ldp)), but some of these legacy systems are still in use, even though they're no longer actively maintained.


## LDP Web Server

Hosts the LDP portal site (`ldp.uchicago.edu`).


## LDP FileMaker Server

Hosts the LDP filemaker server (`ldpdb.spc.uchicago.edu`)


## LDP File Server

Hosts the LDP file server (`ldpfs.spc.uchicago.edu`), accessible via SAMBA on the psych building's subnet.


## LDP FS Backup

This is an offsite backup system (`ldp-backup.spc.uchicago.edu`).  It mirrors the LDP file server (`ldpfs.spc.uchicago.edu`) using `rsync` for the purposes of emergency data recovery.  

As of March 2015 this machine is now located in Susan Goldin-Meadow's new office, as is the backup system for the Goldin-Meadow Lab.


## SGM Lab Server

This is the Goldin-Meadow Lab's file server (`sgmlab.spc.uchicago.edu`), also accessible via SAMBA on the psych building's subnet.


## SGM Lab Backup

This is an offsite backup system (`sgmlab-offsite.spc.uchicago.edu`).  It mirrors the Goldin-Meadow Lab's file server (`sgmlab.spc.uchicago.edu`) using `rsync` for the purposes of emergency data recovery.  

As of March 2015 this machine is now located in Susan Goldin-Meadow's new office, as is the backup system for the LDP file server.


## SPSS Host

This is a Mac mini with SPSS client (`spss.spc.uchicago.edu`).  Anyone needing to use SPSS can `vnc` to the machine to run their analyses.
