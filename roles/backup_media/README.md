Backup media
=========

In this role, the container id is taken from the container name. Then the media files are archived directly in the Django bundle container and sent to the host, then to the storage location by the inveker. After sending, the archive is deleted in the container and on the host.

Requirements
------------

If you setup variables in main-playbook it should be work.

Example Playbook
----------------

~~~bash
ansbile-playbook -i hosts.yaml main-playbook.yaml --ask-become-pass --tags=backup_media
~~~

License
-------

BSD
