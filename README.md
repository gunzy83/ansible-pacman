Ansible-Pacman
==============

**ansible-pacman** is a fork of the offical pacman module for **[Ansible](https://github.com/ansible/ansible)**. The purpose of this repo is to add features to the module for my personal use (and other that clone this repo). I hope that many of these features will be accepted upstream. Original authors of the module are credited below.

Usage
=====

Installing
----------

To use this module simply clone this repository into your library folder:

    $ cd library/
    $ git clone https://github.com/gunzy83/ansible-pacman.git

Example Plays (New features only)
----------------------------

    - name: Ensure bar is installed as a dependency
      pacman:
        name: bar
        state: present
        as_deps: yes

Future Plans
============

* Support force option
* Support package groups (--needed, detect changes)
* Support upgrade (-Syu) with pacnew and pacsave detection
* Submit features to Ansible Extra Modules repository

License
=======

ansible-pacman is provided under the same license as Ansible (GNU General Public License Version 3)

- Copyright © 2012, Afterburn <http://github.com/afterburn>
- Copyright © 2013, Aaron Bull Schaefer <aaron@elasticdog.com>
- Copyright © 2015, Ross Williams