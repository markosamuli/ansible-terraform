# ansible-terraform

[![Build Status](https://travis-ci.org/markosamuli/ansible-terraform.svg?branch=master)](https://travis-ci.org/markosamuli/ansible-terraform)

Ansible role toi nstall [Terraform](https://www.hashicorp.com/) on Ubuntu and macOS.

Used in the Ansible playbooks for setting up my workstations:

- [markosamuli/machine](https://github.com/markosamuli/machine)
- [markosamuli/linux-machine](https://github.com/markosamuli/linux-machine)
- [markosamuli/macos-machine](https://github.com/markosamuli/macos-machine)

## macOS

On macOS, Homebrew [terraform formula](https://formulae.brew.sh/formula/terraform) is used.

## Linux

On Ubuntu, terraform binary is installed into `/opt/terraform` and symlink created
in `/usr/local/bin`.

To change installed version, update the version and checksum:

```yaml
terraform_version: "0.11.10"
terraform_checksum: "sha256:43543a0e56e31b0952ea3623521917e060f2718ab06fe2b2d506cfaa14d54527"
```

See [Terraform Downloads](https://www.terraform.io/downloads.html) page for latest
version.

## License

MIT
