Ansible Role: Upgrade Powershell
================================

An ansible role to upgrade Windows PowerShell to version 5.1.

It uses Chocolatey to upgrade PowerShell and Windows task scheduler to launch the
upgrade after a reboot. It allows to not break Ansible WinRM connection during the process.

Compatibility
-------------

This role is compatible with Windows version:
 - Windows Server 2008 x64
 - Windows Server 2008 R2
 - Windows Server 2012
 - Windows Server 2012 R2

 Current version of PowerShell is checked before the upgrade. If version is not 3.0, 4.0 or
 5.0, nothing is changed.

Role Variables
--------------

No variable should be changed.

Dependencies
------------

No dependency.

Example Playbook
----------------

    - hosts: windows_servers
      roles:
         - role: jpmat296.upgrade_powershell

License
-------

BSD

Author Information
------------------

This role was created in 2020 by [Jean-Pierre Matsumoto](https://fr.linkedin.com/in/jpmatsumoto).
