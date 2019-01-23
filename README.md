# Docker ZFS patches

This coollection of patches addresses performance issues with building
Docker containers on ZFS filesystems (e.g. under FreeBSD). Use of ZFS
native diffing capabilities when generating layers reduces per-layer
build times when the container grows large.

The patches can be of general interest to container-related projects
implemented in Go and supporting ZFS
(e.g. [Jetpack](https://github.com/3ofcoins/jetpack/)).

Patches date back to 2015; back then, Moby was Docker. They apply to
[kvasdopil Docker 582db78c](https://github.com/kvasdopil/docker/commit/582db78ceedc54387386f9b090e90da6624a97ef).

# License

Copyright 2015 Digital Loggers, Inc.

Licensed under the same license as Docker (Apache 2.0).  See the
[LICENSE](LICENSE) file for details.
