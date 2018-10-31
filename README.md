ansible-fusioninventoryagent
============================

- Installs `fusioninventory-agent`
- nightly cronjob to run inventory, and sent it to a GLPI instance

(i.e. passive, not as a deamon).

Currently tested with Debian Stretch, and CentOS6/7.

Example Playbook
----------------


    - hosts: myhosts
      become: true

      vars:
        fusioninventoryagent_server_url: https://glpi.host.org/glpi/plugins/fusioninventory/
        fusioninventoryagent_user: username
        fusioninventoryagent_password: hackme

      roles:
        - ansible-fusioninventoryagent

License
-------

BSD

Author Information
------------------

Dick Visser <dick.visser@geant.org>