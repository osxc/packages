packages
========

Install packages on your mac from different sources

[![Build Status](https://travis-ci.org/osxc/packages.svg)](https://travis-ci.org/osxc/packages/)

## Requirements

the same as the ones required by the dependencies

## Role variables

| Name                  | Description                                      | Default            |
|-----------------------|--------------------------------------------------|--------------------|
| `packages`            | The list of packages to install                  | `[]`               |
| `brew_taps`           | The brew taps you need to open before install    | `[]`               |

### Package variables

| Name                  | Description                                      | Default            |
|-----------------------|--------------------------------------------------|--------------------|
| `name`                | The name of this package                         | none, required     |
| `type`                | The package manager you need to use              | `brew`             |

Available package managers:

- `brew`
- `cask`

## Dependencies

- `osxc.homebrew`

## License

MIT

## Author

- Robin Ricard

