Role Name
=========

Install prometheus node exporter as a service on linux host

Requirements
------------

Linux systems 

Role Variables
--------------
configurable variables for the roles and default values

exporter_port: 9100   -> listening port 
node_exporter_version: 1.1.2 -> exporter version to be installed
node_exporter_user: node_exporter -> user running the service 
node_exporter_group: node_exporter -> user's group
service_directory: /etc/systemd/system -> service directory path
exporter_extra_options: [] -> additional arguments for exporter execution.

Dependencies
------------
None 

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: node-exporter, exporter_extra_options: ["--collector.systemd"] }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
