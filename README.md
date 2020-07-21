![](https://churrops.files.wordpress.com/2017/06/ansible-logo.png?w=736)

# ADD GLOBAL ENVIRONMENT VARIABLE FOR LINUX

- settings hosts
- add host and playbook
- add file in the roles/file directory

### after running the playbook:

There is no need to restart the server, variable is added automatically, but when the equipment is restarted, the variable is added automatically by profile.d


- don't forget to configure the export.sh file with your desired variable.

command to perform test (example):

~~~bash
$ ansible portal -m shell -a 'echo $USR'
[WARNING]: log file at /var/log/ansible.log is not writeable and we cannot create it, aborting 
portal | CHANGED | rc=0 >>
usr_mysql
~~~
