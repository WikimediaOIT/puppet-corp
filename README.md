# puppet-corp
Public puppet repository

WMF Puppet Project Plan
  1. Create private git repository--DONE
  2. Create public git repository--DONE
  3. Build new corporate puppet server
  4. Configure node baseline and modules
    1. ntp
    2. git?
    3. apt-get updates
    4. unattended upgrades
    5. apt-get autoremove
    6. Large /boot partition?
  5. Configure nodes with modules
    1. samba
      1. puppet module install ajjahn-samba
        1. Modify to work with ldap by forking
      2. Needs libnss-ldap
        1. No existing puppet module, needs to be installed with puppet some how?
          1. Found package can be installed via node classification
          2. Module available to manage nsswitch.conf
          3. Module to configure ldap client?
      3. Modify etc/ssh/sshd_config to drop to no shell
    2. icinga
    3. ldap
    4. backup
    5. freeradius
