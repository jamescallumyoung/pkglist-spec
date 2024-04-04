# pkglist-spec

This repository conatins the specification for the pkglist format. This format defines `.pkglist` files, which can be used to install multiple packages at once, with supported package managers.

## The Specification

The specification is defined in [specification.md](./specification.md).

## Rationale

The pkglist format aims to provide a convenient method to install numerous packages on a Linux or macOS system.

The format is inspired by the [Brewfile](https://docs.brew.sh/Manpage#bundle-subcommand) format used by Homebrew, and the [Gemfile](https://bundler.io/guides/gemfile.html) format used by Ruby.

pkglist does not specify how the package manager should operate. It aims only to provide a method to list the packages that should be installed. How this list is interpreted by the package manager is out-of-scope.

## Author & Licence

pkglist was devised by [@jamescallumyoung](https://github.com/jamescallumyoung).

Contributions to this specification are welcome.

The pkglist Specification © 2024 by James Young is licensed under CC BY-SA 4.0. To view a copy of this license, visit [creativecommons.org/licenses/by-sa/4.0](http://creativecommons.org/licenses/by-sa/4.0/).

