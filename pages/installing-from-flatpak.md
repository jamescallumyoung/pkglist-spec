# Installing from `flatpak`

## Packages

`.pkglist` files can specify packages to be installed by `flatpak`.

The prefix for Flatpak packages is `flatpak`.

The package identifier for Flatpak packages is defined by `flatpak` and is
usually one of:

- the package's "Flatpak identifier" - e.g. `com.company.App`
- the package's "Flatpak identifier triple" -- e.g. `com.company.App/i386/stable`
- a URL to a `.flatpakref` file -- e.g. `https://flathub.org/repo/appstream/com.company.App.flatpakref`

Any package identifier that is recognized by `flatpak install` is supported.
See the Flatpak docs for more information on Flatpak's [indentifiers][1],
[identifier triples][2], and the [`.flatpakref`][3] file format.

Note: It is only possible to specify which remote a package should be installed
from by using a `.flatpakref` as the package identifier.

