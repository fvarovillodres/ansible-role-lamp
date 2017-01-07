# Ansible Role: LAMP
=========

Simple instalation of a LAMP stack on Debian/Ubuntu

## Instalation
------------

$ ansible-galaxy install fvarovillodres.lamp

## Requirements

No special requirements; note that this role requires root access, so either run it in a playbook with a global `become: yes`, or invoke the role in your playbook like:

    - hosts: database
      roles:
        - role: fvarovillodres.lamp
          become: yes

## Role Variables
--------------

You can change the document root of Apache in `vars/main.yml` . If you use Ubuntu 16.04 or higher, you should change php5 packages for php in `tasks/php.yml`. You are free to change any part of the rol and adapt it to your needs

## Example Playbook
----------------

    - hosts: all
      become: yes
      roles:
        - fvarovillodres.lamp

## Author Information
------------------

Francisco M Varo Villodres student of SysAdmin in Málaga, Spain.
