Ansible make backup
=========

This is an ansible project where you can take a backup of the postgressql database and mediafile in a Django project that is in a Docker container. The file is then archived and uploaded to your chosen storage location.

Requirements
------------

This script works with another project in my profile called ansible-start-server. In which the containers are created:

1. django project
2. nginx
3. db postgress

Therefore if you run it in another environment you should check if it is compatible with your environment.

Role Variables
--------------

Before running the script you should change:

1. Path to id_ed25519.
2. Path to the backup directory.
3. Path to the invoker backup directory.
4. Check the README files of the roles what else needs to be changed.

Example of use
----------------

~~~bash
ansible-playbook -i host.yml main_playbook.yml --ask-become-pass
~~~

License
-------

BSD
