Php fpm
=========

Ansible role for installing and configure php fpm, php cli and configure php fpm pool. Tested platforms are:
* Debian 8

Requirements
------------

Debian 8 (jessie)

Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

| Parameter | Required | Default | Choices | Comments |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| default_timezone | yes | Europe/Kiev | | Sets default system timezone |
| default_upload_max_filesize | yes | 4 | | Sets max upload file size |
| default_php_user | yes | user | | Sets php process user |
| default_php_group | yes | user | | Set php process user group |
| default_php_memory_limit | yes | 128 | | Set max memory usage per script |

Dependencies
------------

None

Example 
----------------
    ---
    - hosts: all
      roles:
         - { role: antonchernik.php-fpm }

License
-------

MIT / BSD

Author Information
------------------

This role was created in 2017 by [Anton Chernik](https://github.com/antonchernik).
