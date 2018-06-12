Ansible Role: YUM cron
======================

An Ansible role for yum-cron and auto updates confg.

Requirements
------------

None.

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

    yumcron_update_cmd: default
    yumcron_update_messages: 'yes'
    yumcron_download_updates: 'yes'
    yumcron_apply_updates: 'no'
    yumcron_random_sleep: 360
    yumcron_system_name: None
    yumcron_emit_via: stdio
    yumcron_output_width: 80
    yumcron_email_from: root@localhost
    yumcron_email_to:
      - root
    yumcron_email_host: localhost
    yumcron_group_list: None
    yumcron_group_package_types:
      - mandatory
      - default
    yumcron_debuglevel: -2
    # yumcron_skip_broken: 'True'
    yumcron_mdpolicy: group:main
    # yumcron_assumeyes: 'True'

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      roles:
         - yum-cron

License
-------

BSD

Author Information
------------------

This role was created in 2018 by [Aymeric Bringard](https://github.com/diadzine).
