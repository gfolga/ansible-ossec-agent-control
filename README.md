ossec-agent-control for Ansible
=================

A role for controlling [OSSEC](http://ossec.github.io/) agents via [Wazuh RESTful API](http://wazuh-documentation.readthedocs.io/en/latest/ossec_api.html) using [Ansible](http://www.ansibleworks.com/).


Usage
-----

Clone this repo into your roles directory:

    $ git clone https://github.com/gfolga/ansible-ossec-agent-control.git roles/ossec-agent-control

And add it to your play's roles:

    - hosts: ...
      vars:
        - restart: True
        - syscheck: True
        - cleardb: False
      roles:
        - ossec-agent-control
        - ...


Changelog
---------

### 0.1

Initial version.
