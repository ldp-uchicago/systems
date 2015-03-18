# Legacy Systems

The LDP once had a database and sys admin named Ben Trofatter (2007-2015) before he moved onto work for Google.  He originally setup and maintained a number of machines for the LDP, SILC, and the Goldin-Meadow Lab.

Below is a list of systems Ben had setup and maintained.


## LDP Web Server

Hosts the LDP portal site (`ldp.uchicago.edu`).


## LDP FileMaker Server

Hosts the LDP filemaker server (`ldpdb.spc.uchicago.edu`)


## LDP File Server

Hosts the LDP file server (`ldpfs.spc.uchicago.edu`).  The file server is accessible via SAMBA on the psych building's subnet.


## LDP FS Backup

This is an offsite backup system (`ldp-backup.spc.uchicago.edu`).  It mirrors the LDP file server (`ldpfs.spc.uchicago.edu`) using `rsync` for the purposes of emergency data recovery.  

As of March 2015 this machine is now located in Susan Goldin-Meadow's new office, as is the backup system for the Goldin-Meadow Lab.


## SGM Lab Server

This is the Goldin-Meadow Lab's file server (`sgmlab.spc.uchicago.edu`).  It's also accessible via SAMBA on the psych building's subnet.


## SGM Lab Backup

This is an offsite backup system (`sgmlab-offsite.spc.uchicago.edu`).  It mirrors the Goldin-Meadow Lab's file server (`sgmlab.spc.uchicago.edu`) using `rsync` for the purposes of emergency data recovery.  

As of March 2015 this machine is now located in Susan Goldin-Meadow's new office, as is the backup system for the LDP file server.


## SPSS Host

This is a Mac mini with SPSS client (`spss.spc.uchicago.edu`).  Anyone needing to use SPSS can `vnc` to the machine to run their analyses.
