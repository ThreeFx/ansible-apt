apt
=========

Configures apt.

Requirements
------------

An apt-based host to configure.

Role Variables
--------------


| Variable Name | Default Value | Description |
--------------- |---------------|--------------
`apt_install_recommends` | "true" | Whether to install recommended packages. Should be a string variable.
`apt_install_suggests` | "false" | Whether to install suggested packages. Should be a string variable.
`apt_additional_keys` | [] | Additional APT keys to install. Must include GPG files (beginning with `----- BEGIN PUBLIC KEY -----`)
`apt_additional_repositories` | [] | Additional repositories to configure. [Debian guidelines apply](https://wiki.debian.org/DontBreakDebian)
`apt_pins` | [] | Package pins to configure, see `defaults/main.yml` for more information

Dependencies
------------

None.

Example Playbook
----------------

See `molecule/default/playbook.yml`.

License
-------

BSD

Author Information
------------------

Find me on [GitHub](https://github.com/ThreeFx).
