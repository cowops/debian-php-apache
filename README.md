Debian-PHP-Apache
===================

Apache 2 PHP Module

Requirements
------------

This role requires a debian compliant system such as ubuntu.

Role Variables
--------------

debian:
    version: wheezy
    locale: fr_FR.UTF-8
    mirror: ftp.fr.debian.org
php:
    timezone: "Europe/Paris"

Dependencies
------------

Apache2

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: cowops.debian-php-apache, debian.version: wheezy, debian.locale: fr_FR.UTF-8, debian.mirror: ftp.fr.debian.org, php.timezone: "Europe/Paris" }

Tasks
-----

  - Install [php](http://www.php.net/manual/fr/install.unix.apache2.php)
  - Setup with default php.ini

License
-------

BSD
