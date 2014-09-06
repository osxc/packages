packages
========

Install packages on your mac from different sources

[![Build Status](https://travis-ci.org/osxc/packages.svg)](https://travis-ci.org/osxc/packages/)

## Requirements

the same as the ones required by the dependencies

## Role variables

| Name                  | Description                                      | Default            |
|-----------------------|--------------------------------------------------|--------------------|
| `brew_packages`       | The list of the homebrew packages to install     | `[]`               |
| `cask_packages`       | The list of the cask packages to install         | `[]`               |
| `brew_taps`           | The brew taps you need to open before install    | `[]`               |

## Dependencies

- `osxc.homebrew`

## License

MIT

## Author

- Robin Ricard

