Role Name
=========

This role automates the process of installing the necessary YottaDB-apiserver service to allow integration with Infinity/Grafana.

Requirements
------------

It is assumed that Yottadb is aready installed on the server as well as Grafana and the Infinity datasource.

Role Variables
--------------

instdir - The directory in which YottaDB-dashboard is to be installed

[ Default - /usr/local/YottaDB-dashboard ]


yotta_env - Environmental variables when running service process

[ Defaults - 
       YOTTA_API_PORT: '8002'
       YOTTA_API_SERVER: '0.0.0.0'
       yotta_dir: '/root/.yottadb/r1.30_x86_64' ]
       yotta_instdir: '/usr/local/Yotta-dashboard'
       ydb_dir: '/root/.yottadb/r1.30_x86_64'
       ydb_rel: 'r1.30_x86_64'
       ydb_gbl: '/root/.yottadb/r1.30_x86_64/g/yottadb' ]

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      role: YottaDB-apiserver
      instdir: /opt/YottaDB-dashboard
      ...

Further Information
-------------------

The git repo referenced in the role to install the dashboard:

https://github.com/RamSailopal/YottaDB-dashboard

License
-------

BSD

Author Information
------------------

Raman Sailopal
