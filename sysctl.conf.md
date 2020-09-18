# Changes to network stack on host required currently for podman

# Add ability for rootless containers to attach to ports <1024, E.G. port 80
`net.ipv4.ip_unprivileged_port_start=0`

# Add so podman containers can ping each other - suggest remove before production
`net.ipv4.ping_group_range=0 2000000`
