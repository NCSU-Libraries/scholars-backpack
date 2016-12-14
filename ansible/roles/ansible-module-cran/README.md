ansible-module-cran
=========

An ansible module to install/uninstall R packages

Requirements
------------

- R


Installation
------------

Install from [Ansible Garaxy](https://galaxy.ansible.com/):

    ansible-galaxy install yutannihilation.module-cran

Or, use this directly:

    ansible-playbook --module-path=/path/to/ansible-module-cran/library your-playbook.yml


Example Playbook
----------------

    - hosts: localhost
      connection: local
      roles:
        - { role: yutannihilation.module-cran }
      tasks:
        - name: install R pakcages
          cran: name={{ item }} state=present
          with_items:
            - dplyr
            - ggplot2
            - purrr
            - tidyr

License
-------

MIT
