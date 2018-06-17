# Ansible Role for Chocolately.Server
This is a simple Ansible role to configure an instance of Chocolately.Server.

Tasks run are based on instructions from [chocolately.org](https://chocolatey.org/docs/how-to-set-up-chocolatey-server).

Role Variables
--------------

The final task looks for a variable value for the API key used to push packages.

    chocolatey_api: MyAPIKey

Example Playbook
----------------

    - hosts: win_servers
      roles:
         - role: gyamada619.chocoserver
           chocolatey_api: MyAPIKey

Requirements
------------

The user running this role needs administrator access.

* Windows 7+ / Windows Server 2008+
* PowerShell v3+
* .NET Framework 4+ (the installation will attempt to install .NET 4.0 if you do not have it installed)

Dependencies
------------

None.

License
-------

MIT
