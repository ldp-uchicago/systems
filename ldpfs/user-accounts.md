# `ldpfs` user accounts

This is an overview of the process for setting up user accounts on the LDP's
file server (`ldpfs.spc.uchicago.edu`).

The video server is a FreeBSD box, so you can use `adduser` command for adding 
new unix accounts and `smbpasswd` to add a new samba account or change an existing users password.

To manage accounts and keep them in sync, use the scripts in `/usr/local/scripts`.  Use `add-ldp-user` to add an account and `rm-ldp-user USERNAME` to remove.

The former will prompt you for the new user's name, username, and password.  
The password must be entered the same way twice for the script to complete 
and the user to be created.
