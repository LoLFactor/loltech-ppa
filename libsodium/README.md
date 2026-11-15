# Libsodium packaging rules

I based these off the Debian packaging rules for libsodium, which can be seen [here](https://sources.debian.org/src/libsodium/1.0.22-2/debian).

I only modified the `control` file to change the source name and `-dev` package name, and the `-dev.install` file to change the installation directories.

Both these modifications were made in the name of coexistence with the OS-supplied version of libsodium on Ubuntu 26.04, which is `lobsodium23`, version `1.0.18`.

I also changed the `source/format` from `quilt` to `native` so I can use my desired versioning scheme.
