# Ansible role for sensible LAMP stack

The official Apache2 package for Ubuntu has some pretty barebone default settings:

- `sites-enabled/` directory not included.
- A dull "It works!" index page.
- `rewrite` module disabled.
- No favicon.ico

This Ansible Galaxy role addresses the above, plus installing the MySQL and PHP5 packages, providing a more sensible LAMP stack installation.

## Requirements

Ubuntu 12.04 or later, including [elementaryOS][eos] 0.2 "Luna".

## Installation

    $ ansible-galaxy install vivaserver.ansible-lamp 

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - vivaserver.ansible-lamp

## License

MIT

## Copyright

(c)2014 Cristian R. Arroyo

[eos]: http://elementaryos.org
