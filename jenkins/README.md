Role Name
=========

This Role is designed to installed jenkins as service on linux hosts

Requirements
------------

Linux redhad or Debian based systems

Role Variables
--------------

allows custom configuration of jenkins service. 
default values for following variable can be overriten when installing the role.
JENKINS_PORT: 8080
JENKINS_HOME: /var/lib/jenkins
JENKINS_CONFIG_DIR: /etc/systemd/system/jenkins.service.d/


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: jenkins, JENKINS_PORT: 8081 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
