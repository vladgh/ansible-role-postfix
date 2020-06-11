# Ansible Role: Postfix

![Build Status](https://github.com/vladgh/ansible-role-postfix/workflows/CI/badge.svg)
[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](code_of_conduct.md)

Vlad's Postfix Ansible Role to set up a Postfix server in Debian-like systems. It has a minimal configuration and is intended to be just a simple relay server using SendGrid or GMail.

## Requirements

*_N/A_*

## Role Variables

Available variables are listed below, along with default values (see defaults/main.yml):

- `smtp_server_address`: The address of the SMTP server
- `smtp_server_port`: The port of the SMTP server
- `smtp_user`: The SMTP user
- `smtp_password`: The SMTP password

## Dependencies

*_N/A_*

## Example Playbook

```yaml
- hosts: all
  become: yes
  roles:
    - vladgh.postfix
```

## Contribute

Contributions are always welcome! Please read the [contribution guidelines](.github/CONTRIBUTING.md) and the [code of conduct](.github/CODE_OF_CONDUCT.md).

## License

Licensed under the Apache License, Version 2.0.
See [LICENSE](LICENSE) file.
