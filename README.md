# Ansible Role: db_iiq_mysql_remove
Remove a Docker instance of MySQL provisioned for an IdentityIQ sandbox

## Requirements

You must have Docker installed and MySQL deployed.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    db_volume_name: sandbox_iiq_db_data

Name of the volume for the MySQL data directory.  Usually overriden in the format of <company name>_iiq_db_data

    db_container_name: sandbox_iiq_db

Name of the MySQL container.  Usually overriden in the format of <company name>_iiq_db

    network_name: sandbox_iiq
    
Name of the docker network to attach the generated containers to.  Usually overriden in the format of <company name>_iiq

    remove: false

Flag to determine if the accelerator pack is being installed.

## Dependencies

None.