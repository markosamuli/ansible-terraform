# markosamuli.terraform

[![GitHub release](https://img.shields.io/github/release/markosamuli/ansible-terraform.svg)](https://github.com/markosamuli/ansible-terraform/releases)
[![License](https://img.shields.io/github/license/markosamuli/ansible-terraform.svg)](https://github.com/markosamuli/ansible-terraform/blob/master/LICENSE)

| Branch  | Status |
|---------|--------|
| master  | [![Build Status](https://travis-ci.org/markosamuli/ansible-terraform.svg?branch=master)](https://travis-ci.org/markosamuli/ansible-terraform)
| develop | [![Build Status](https://travis-ci.org/markosamuli/ansible-terraform.svg?branch=develop)](https://travis-ci.org/markosamuli/ansible-terraform)

Ansible role to install [Terraform] on Ubuntu and macOS.

Used in the Ansible playbooks for setting up my workstations:

- [markosamuli/machine](https://github.com/markosamuli/machine)
- [markosamuli/linux-machine](https://github.com/markosamuli/linux-machine)
- [markosamuli/macos-machine](https://github.com/markosamuli/macos-machine)

[Terraform]: https://www.hashicorp.com/

## macOS

On macOS, Homebrew [terraform formula] is used.

[terraform formula]: https://formulae.brew.sh/formula/terraform

## Linux

On Linux, the `terraform` binary is installed into `/opt/terraform/<version>`
and a symlink is created in `/usr/local/bin`.

## Updating version

To update Linux version, run the `update-release` script:

```bash
./update-release
```

See [Terraform Downloads] page for latest version.

[Terraform Downloads]: https://www.terraform.io/downloads.html

## License

- [MIT](LICENSE)

## Author Information

- [@markosamuli](https://github.com/markosamuli)
