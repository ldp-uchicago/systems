# Disk Issues

One of the backup systems is not booting into multi-user mode and appears to
file system issues and perhaps a corrputed disk.

We're going to try using [`fsck`](https://www.freebsd.org/cgi/man.cgi?query=fsck) (a basic utility for doing file system checks) to do a consistency check and interactive repair of your disk partitions.

See [this forum thread](https://forums.freebsd.org/threads/best-way-to-check-and-fix-corrupt-disk.1823/) for recommendations on the best way to check and fix a corrupt disk.  

The main recommendation is to first try running `fsck -y` after [booting into single-user mode](https://www.freebsd.org/doc/handbook/boot-introduction.html#boot-singleuser) in order to check and fix the file system of each mountable partition. (If there's a problem with a file system you'll likely boot into single-user mode by default.) To see a list of mountable file systems run the `mount` command (or `cat /etc/fstab`).
