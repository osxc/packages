packages
========

Install packages on your mac from different sources

[![Build Status](https://travis-ci.org/osxc/packages.svg)](https://travis-ci.org/osxc/packages/)

## Requirements

the same as the ones required by the dependencies

## Role variables
the following are all **optional** and can be applied only as needed:

| Name                  | Description                                      | Default            |
|-----------------------|--------------------------------------------------|--------------------|
| `brew_taps`           | The brew taps you need to open before install    | `[]`               |
| `brew_packages`       | The list of the homebrew packages to install     | `[]`               |
| `cask_packages`       | The list of the cask packages to install         | `[]`               |
| `brew_pkg_with_opts`  | A dict of homebrew packages to install with the  |                    |
|                       | options seperated by commas, see example below   |                    |

## Playbook example
```YAML
---

- hosts: all
  roles:
  - role: osxc.packages
    brew_taps:
    - caskroom/fonts
    brew_packages:
    - git
    - zsh
    cask_packages:
    - font-inconsolata
    brew_pkg_with_opts:
    - { pkg: "curl" , opts: "with-idn,with-openssl" }

```
## Dependencies

- `osxc.homebrew`

## License

MIT

## Author

- Robin Ricard

