# Guacamole

## Initial Setup

On the "guacamole" container, run:
``

On the "mysql" container, run:
`cat /setup/initdb.sql | mysql -u root -p guacamole_db`

## Post-Installation

Make sure you create your own user account and delete the "guacadmin" user (or at very least change the password)

## TODO
* Allow adding extensions