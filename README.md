# Ansible role for a sensible LAMP stack

![screenshot](https://raw.github.com/vivaserver/ansible-lamp/master/screenshot.png)

The official Apache2 package for Ubuntu has some pretty barebone default settings:

- ["Could not reliably determine the server's fully qualified domain name"][bug] warning.
- `sites-enabled/` directory not included.
- A dull "It works!" index page.
- `rewrite` module disabled.
- No favicon.ico

This Ansible Galaxy role addresses the above, plus installing the MySQL and PHP5 packages, providing a more sensible LAMP stack installation.

## Requirements

Ubuntu 12.04 or later, including [elementaryOS][eos] 0.2 "Luna".

## Installation

    $ ansible-galaxy install vivaserver.lamp 

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - vivaserver.lamp

## License

MIT

## Copyright

(c)2014 Cristian R. Arroyo

[bug]: http://askubuntu.com/questions/256013/could-not-reliably-determine-the-servers-fully-qualified-domain-name
[eos]: http://elementaryos.org
