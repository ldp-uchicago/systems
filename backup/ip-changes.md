# IP Address Changes

The backup machines for the LDP and SGM Lab file servers were assigned new IP addresses in Feb 2015.  See Laura Tharsen or Bart Longacre for details.

    hostname                sgmlab-offsite.spc.uchicago.edu
    ip address              128.135.47.92
    subnet mask             255.255.255.0
    gateway/default router  128.135.47.1

    hostname                ldp-backup.spc.uchicago.edu
    ip address              128.135.47.77
    subnet mask             255.255.255.0
    gateway/default router  128.135.47.1

Jason Voigt provided Kristi Schonwald with the instructions below for updating the network configuration on both machines.

---

Run `ifconfig` to view current configuration of the system's [network interfaces](https://www.freebsd.org/doc/en_US.ISO8859-1/articles/linux-users/network.html).

Modify the existing IP configuration in `/etc/rc.conf`:

    hostname="ldp-backup.spc.uchicago.edu"
    // change previous address `128.135.143.60` to ...
    ifconfig_em0="inet 128.135.47.77 netmask 255.255.255.0"
    // change defaultrouter `128.135.143.1` to ...
    defaultrouter="128.135.47.1"

    hostname="sgmlab-offsite.spc.uchicago.edu"
    // change previous address `128.135.143.84` to ...
    ifconfig_em0="inet 128.135.47.92 netmask 255.255.255.0"
    // change defaultrouter `128.135.143.1` to ...
    defaultrouter="128.135.47.1"

Then, restart the network and routing services:

    # /etc/rc.d/netif restart && /etc/rc.d/routing restart

See [this article](http://www.cyberciti.biz/tips/freebsd-how-to-start-restart-stop-network-service.html) for details on restarting freebsd networking services.
