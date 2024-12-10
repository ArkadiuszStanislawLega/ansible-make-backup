Backup postgress
=========

In this role, a place for a backup dump is created if it has not been created before. Then a dump is made from the database to an sql file. The file is transferred from the docker container to the host, and then sent to the inveker.

Requirements
------------

To run this role, you need to change the variables for the database.

Role Variables
--------------

1. db_docker_container - name of the docker container with postgressql
2. db_user - user name to enter to database
3. db_name - the name of the database from which the backup will be created

Example Playbook
----------------

~~~bash
ansbile-playbook -i hosts.yaml main-playbook.yaml --ask-become-pass --tags=backup_postgress
~~~

License
-------

BSD
