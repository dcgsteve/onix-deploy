# onix-deploy

A set of scripts to help deploy out a local development version of Onix.

In order for rootless pods to utilise ports less than 1024, you will need to amend the host network stack to allow this. Add the following line to your `sysctl.conf`:

`net.ipv4.ip_unprivileged_port_start=0`
