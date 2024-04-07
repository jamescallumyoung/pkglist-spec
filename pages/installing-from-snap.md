# Installing from `snap`

## Packages

`.pkglist` files can specify packages to be installed by `snap`.

Snap allows packages to be installed in different "[modes][1]".
These modes provide different levels of software isolation.

pkglist supports two modes for Snap: the default mode, and classic mode.
The mode can be selected by using the appropriate prefix:

- `snap` for default mode
- `snap-classic` for classic mode

The package identifier for Snap packages is defined by `snap`,
and is just the package's name - e.g. `blender`.

Any package identifier that is recognized by `snap install` is supported.

Note: It is not possible to specify which channel a package should be installed from.

