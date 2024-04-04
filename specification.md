# The pkglist Specification

This specification defines two types of content:

- package entries,
- and comments.

A pkglist file is valid so long as it contains only package entries, comments, or empty lines.

## Package Entries

A package entry is a line in the pkglist that defines a package that should be installed.

Package entreis have two parts: a prefix, and a package identifier. Both parts are required. They are formatted as follows:

```
prefix package-identifier
```

### Prefixes

Prefixes identify the package manager that should be used to install the package. In some cases, they also identify additional options that should be used when installing the package.

Currently supported prefixes are limited to:

- `apt` for packages installable by [APT](https://en.wikipedia.org/wiki/APT_(software)).
- `flatpak` for packages installable by [Flatpak](https://flatpak.org/).
- `snap` for packages installable by [Snap](https://snapcraft.io/about), using the default install mode.
- `snap-classic` for packages installable by Snap, using the [classic](https://snapcraft.io/docs/install-modes#heading--classic) install mode.

Prefixes should be followed by a whitespace character to seperate them from the package identifier.

### Package Identifiers

Package identifiers are, most simply, any string that can uniquely identify a package for installation by the relevant package manager.

The exact format of a package identifier is out-of-scope of pkglist.
Instead, the identifier format is dictated by the package manager that should be used to install the package.

The package identifier must be usable by the package manager to install the package, without further information needing to be specified.

## Comments

A comment is any line that starts with the `#` character.

Comments are whole lines.
A comment cannot be added to the end of a line containing a package entry.

## File Extension

pkglist files should end with the `.pkglist` extension.

