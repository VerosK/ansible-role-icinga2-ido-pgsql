# icinga2-ido-postgres

Ansible role to set-up Icinga2 IDO with postgresql for separated
database amdn monitoring host.

## Requirements

Icinga2 should be present to target host, ideally  
with [`VerosK.icinga`][role] role.

## Example Playbook
    
    - hosts: icinga
      roles:
       - role: VerosK.icinga2
       - role: VerosK.icinga2-ido-postgres
         icinga2_ido_pg_host: postgres


Role Variables
--------------

 `icinga2_ido_pg_host`:  PostgreQQL login host
 
 `icinga2_ido_pg_user`, `icinga2_ido_pg_user`   

License
-------

2-BSD or CC-0


[role]: https://galaxy.ansible.com/VerosK/icinga2/