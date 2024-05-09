Kernel Crash Dump
=========

An ansible role which configures kdump.

Requirements
------------
Ansible 2.4 or higher
Ubuntu 22.04 LTS or equivalent 


Role Variables
--------------
Currently the following variables are supported:

kdump_crash_path - the path in which to store kernel crash dump files
kdump_core_collector_args - parameters/options to pass into the core collector configuration (not configured by default)
kdump_dracut_device - the location of a device to mount onto a specified mountpoint (not configured by default)
kdump_dracut_mountpoint - the location a specified device is to be mounted (not configured by default)
kdump_dracut_filesystem_type - the type of filesystem of the device in its initramfs (not configured by default)
kdump_dracut_filesystem_options - configuration options for the filesystem (not configured by default)

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: ahmam.kdump }

License
-------

BSD

Author Information
------------------

Ahmed Mamlouk ahmed.mamlouk@gmail.com
