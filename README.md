
ansible-role-newrelic-infra
=========

Ansible role for installing and configuring the New Relic Infrastructure Agent

Role Variables
--------------

- `newrelic_infra_license_key`: New Relic license key (this is a required variable)

- `newrelic_infra_repo_script`: Script for configuring package repository (default: `https://75aae388e7629eec895d26b0943bbfd06288356953c5777d:@packagecloud.io/install/repositories/newrelic/infra-beta/script.deb.sh`)

Example Playbook
----------------

    - hosts: all
      become: yes
      roles:
         - role: ansible-role-newrelic-infra
           newrelic_infra_license_key: xxxxxxxxx

Author Information
------------------

[SinglePlatform Engineering](http://engineering.singleplatform.com/)

License
-------

BSD 3-Clause
