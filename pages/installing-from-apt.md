# Installing from `apt`

## Packages

`.pkglist` files can specify packages to be installed by `apt`.

The prefix for APT packages is `apt`.

The package identifier for APT packages is defined by `apt-get`, and is usually
one of:

- the package's name - e.g. `git`
- the package's name, plus a version -- e.g. `git=1:2.34.1-1ubuntu1.10`

Any package identifier that is recognized by `apt install` is supported.

Note: It is not possible to specify which repository a package should be installed from.

