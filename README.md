# bootc

Transactional, in-place operating system updates using OCI/Docker container images.

# Motivation

The original Docker container model of using "layers" to model
applications has been extremely successful.  This project
aims to apply the same technique for bootable host systems - using
standard OCI/Docker containers as a transport and delivery format
for base operating system updates.

The container image includes a Linux kernel (in e.g. `/usr/lib/modules`),
which is used to boot.  At runtime on a target system, the base userspace is
*not* itself running in a container by default.  For example, assuming
systemd is in use, systemd acts as pid1 as usual - there's no "outer" process.

# Status

NOTE: At the current time, bootc has not reached 1.0, and it is possible
that some APIs and CLIs may change.

# More information

See the [project documentation](https://containers.github.io/bootc/).


extra docs


more docs


moar tests