EWC Ansible Role Conda
======================

Install Conda package manager. By default, it will use [Miniforge](https://github.com/conda-forge/miniforge) installer.

Requirements
------------
None

Role Variables
--------------
 - `conda_installer`: URI of the installer to use. Default: `https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-Linux-x86_64.sh`
 - `conda_prefix`: Prefix where conda will be installed. Default: `/opt/conda`
 - `conda_update_base`: Boolean to decide wether base environment needs updating. Default: `false`
 - `conda_user`: User that will own the conda installation. Default: `root`

Example Playbook
----------------

    - hosts: all
      roles:
         -  ewc-ansible-role-conda

License
-------

Apache 2.0.

Author Information
------------------

ECMWF for the European Weather Cloud